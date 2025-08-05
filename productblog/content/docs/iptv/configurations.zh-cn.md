---
title: "配置"
weight: 2
prev: /docs/iptv/get-started
next: /docs/iptv/iptvplus
---

尽管只要您拥有个人 IPTV 提供商，IPTV Fluent 就已准备好播放流媒体，但它仍然提供了强大的自定义设置。

<!--more-->
## 菜单布局

要在 IPTV Fluent 中调整设置，只需点击左侧菜单中的`设置`按钮。

{{< filetree/container >}}
{{< filetree/folder name="IPTV Fluent" state="open">}}
{{< filetree/file name="直播" >}}
{{< filetree/file name="频道" >}}
{{< filetree/file name="播放单" >}}
{{< filetree/file name="设置" >}}
{{< /filetree/folder >}}
{{< /filetree/container >}}

## 常规设置

### 主题

提供自动、浅色、深色三种主题，自动即与设备的主题保持一致。

### 启动菜单

![image](https://od.lk/s/200607426_u0Sx5/launchmenu.png)

有`直播`、`频道`、`播放单`、`媒体中心`和`大屏幕`。启动应用后，它将立即打开您选择的选项。

### 应用语言

![image](https://od.lk/s/200607851_yegn7/language.png)
应用中提供了 21 种语言选项。

除了英语、法语、西班牙语和中文外，其他语言均由 AI 和机器翻译。如果希望帮助我们翻译应用，欢迎加入在 Crowdin 平台的翻译团队。

如果您的操作系统没有相应的语言包，对应的语言则不会显示崽设置中。

## 播放列表同步

![image](https://od.lk/s/200608026_n1oNA/sync.png)

用户添加的在线播放列表和收藏列表可以通过 OneDrive 在桌面和平板电脑等设备之间同步。

您需要手动在设备之间点击上传和下载。自动同步功能正在开发中。

目前此功能仅适用于 IPTV Plus。

## 播放设置

### 播放引擎

![image](https://od.lk/s/200609031_t4bhu/playbackengine.png)

播放引擎是流媒体播放的核心播放器。如果在播放某些直播流时遇到问题，您可以尝试更换播放引擎。

1: VLC：提供更好的图像质量和源支持。

2: 系统：原生播放器在 RAM 内存管理和稳定性管理方面表现更佳。

3: FFMpeg：对流媒体的支持更好，但会消耗更多的 RAM 内存。

### EPG 电子节目指南

![image](https://od.lk/s/200611282_LCp8I/EPG.png)

自定义 EPG 需要一个外部的 xml 链接，该链接可能由您的 IPTV 提供商提供，或者您可以在网上搜索。

![image](https://od.lk/s/200612577_CWt9Q/epg2.png)
设置 URL 后，它将显示即将播放的节目。

### 自动睡眠

![image](https://od.lk/s/200612991_jD6Gx/autosleep.png)
应用支持在一定时间后自动关闭。

## 列表设置

### 默认列表视图

在频道列表中，默认显示为单行列表。

您可以选择 Grid 选项以带节目徽标的方式显示。

### 自动检测延迟

在某些情况下，您可能会从网上获取不可靠的 M3U 列表。

其中的许多频道可能在您的地区不可用。

打开此功能后，加载在线列表后将自动隐藏这些频道。

### 更新频率

选择 `每天` 或 `每月` 选项可以每日或每月缓存在线列表，而无需每次加载列表。

### 更换默认在线地址

除了在左边搜索频道处直接替换，也可以在设置中对默认的在线列表进行修改。

## 阅读更多

- [维基百科：电子节目指南](https://zh.wikipedia.org/wiki/%E7%94%B5%E5%AD%90%E8%8A%82%E7%9B%AE%E6%8C%87%E5%8D%97)
