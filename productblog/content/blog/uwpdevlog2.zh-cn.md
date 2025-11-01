---
title: 记 UWP 应用迁移 .NET 9 踩的坑
date: 2025-09-07
authors:
  - name: JimmyRespawn
    link: https://github.com/JimmyRespawn
    image: https://github.com/JimmyRespawn.png
tags:
  - .NET9
  - UWP
  - devlog
excludeSearch: true
hidden: true
---

又到了久违的 UWP Devlog，最近想把老项目支持 WinUI 2，干脆决定重新创建个新的项目干净的。正好看到去年支持的 UWP .NET 9 在五六月的时候已经正式版，VS2022也内置的模板，那干脆就新建。因为支持 .NET 9 对于 UWP 其实还是挺重要，特别是你比较依赖外部的库做功能的话，无异于可以更好支持自己的项目。至于 AOT 等等，锦上添花。于是创建空项目，率先试了下能不能生成 msixupload 包，毕竟之前遇到过项目总算迁完，结果最后生成包各种傻眼和坑，生产了下成功，信心满满开始编码(拷贝)。其实代码优化本身遇到的问题并不多，99%直接复制过去都可以跑起来。下面是碰到的小坑。

## 开发中遇到的坑

1. 发布包部分功能不执行：Debug下跑的好好的，Release包怎么就功能不行了。有了 WinUI 3 的经验，直接在项目文件里加上<AllowUnsafeBlocks>到true，<PublishAOT>到false，<TrimMode>到false，马上让你纸糊代码焕发新生。这次比较诡异的是PublishTrimmed在Debug下打开会有问题，那加个Configuration在Debug时候设置false，在Release时候设置到true，成功解决所有问题
2. 部分老库不可用：我碰到的是 OneDrive.SDK.Authentication 在 .Net 9 下跑不起来，索性 OneDrive.SDK 还能跑，之前试着迁移到新的 Graph API，因为 UWP 这个历史问题，其实后面创建的包在 Azure 下没有 Id，那么就导致不得不继续用 OneDrive.SDK 了。运气好，凭借强力的 AI，成功实现 Authentication 的授权功能，而且能调起系统弹窗，非常完美的解决。不过每个人可能碰到库不可用的情况不同，所以可能会是给隐形雷。
3. 最终生成要提交的 Store 包失败：VS创建包的时候疯狂提示 WinAppSdkSignAppxPackageBundle 错误，搜了一圈都有这个问题，最后在某语音软件里有人说是 Visual Assets 导致的，我试了下果然是，任何 -100， -125,-150,-400 的图片会导致生成不同分辨率的包，但是神奇的时候 VS 调用 MakeAppx 不知道哪里抽风，最后合包的时候一顿报错。那么把这些后缀的assets图片删了，就能成功生成最终包
4. 生成的 Store 包缺乏多语言：最终生成的包竟然不包括任何其他多语言的文件，msix 包里还有，到 msixbundle 下面的时候全部消失，搜了半天也没看到有人遇到。最后发现要去csproj里加上各种语言节点才能生成在最终上传的包里。
5. 没有 Designer View：最神奇的是，竟然把 Xaml Designer 的视图删了，这玩意儿你说开发多了的人无所谓，但是偶尔要在界面里找到某个节点，Desinger View原来这么成熟，说砍就砍。热加载这玩意儿有时候好用，但还是不如 DV。网上有人调侃 Visual Studio 没有了 Visual。

## .NET9 for UWP 优点

其实在做当中还是发现迁移后还是有很多好处

1. 第三方库支持：不少库要求提的越来越高，不支持老项目。或者有些库能装上，你在用的时候发现有这样那样的Bug，上了 .NET 9 之后神奇的事情发生，有些 bug 自愈了。这无疑是升级的最大好处。
2. AOT裁剪：可以把包裁剪到很小。其他启动时间、内存占用我倒是觉得于 UWP 来说优势不大，毕竟 .Net Native 在 Win 下的启动速度和性能已经是无敌的存在。至今还是有人怀念不少exe把uwp砍了，在商店留差评。
3. C#9.0 支持：恭喜你，可以使用最新版的最好的语言。
4. 未来迁移支持：.NET 9 跳到 WinUI 3 无疑比 UWP 直接跳到 WinUI 3 方便，不过这个优点聊胜于无。

## 结语

在 XAML 部分 .Net9 和 .Native 区别本质不大，毕竟前端就这样了，扒着 WinUI 大腿就完事。但是 UWP 本身开箱开发至今，本身除了打包经常报错外也不像这次版本遇到各种奇怪的坑。虽然 UWP 现在估计拿掉了面向新手的标签。老是要调 csproj 参数属实不是一种新手友好的开箱体验。

其实现在 WinUI 3 一堆新的 API 都盯着 AI 功能，而不是 AI 特性不是要显卡就是要有 NPU，假如 UWP .NET 9 能解决第三点和第五点问题，普通功能的应用再用过个五六年其实问题也不大。毕竟在这个年代，稳定的确是大于一切。不是什么东西都像技术一样，追求新的框架，最终稿呈现在别人面前的还是产品。

以上。
