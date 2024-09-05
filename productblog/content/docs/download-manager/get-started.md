---
title: "Get started"
weight: 1
prev: /docs/download-manager/
next: /docs/download-manager/configrations
---

If you want to learn more about the Download Manager, please take your time to go through the following documentation.

<!--more-->

## 1. How to start downloading

- Method 1: In the "Downloads" tab, click the `+` button at the bottom right or top right corner to directly open a popup where you can input the download link. Simply enter the hyperlink you want to download.

- Method 2: If you prefer to have a popup appear when clicking on downloadable files while browsing, it is recommended to use the in-app browser.

- Method 3: Extensions, currently under development.

## 2. In-app Browser

The Download Manager includes a built-in browser designed for sniffing out downloadable files from complex pages. This prevents scenarios where the default download link might lead to misleading executable files. For detailed usage instructions, see the "In-app Browser" section.

P.S. Don’t worry, this is not a Chromium wrapper; it uses Windows' built-in Edge WebView 2, so it won’t take up additional app space.

P.S.2 Please be aware of the safety of the download platform. DMK itself does not check whether the downloaded file contains threats. Although the system's default antivirus software will scan the file after the download is complete, it may mistakenly associate the downloader with the file.

## 3. File Manager

The app includes a built-in file manager for managing downloaded files, supporting common file management functions such as opening, copying, moving, and renaming. However, it can only manage files within the download folder. Due to UWP sandboxing, files outside the download folder cannot be accessed or managed by the app.

## 4. Application Principle

Advantages: The app uses the .Net Native Download Operation, which means the Download Manager uses truly native download threads, resulting in an extremely lightweight and fast experience.
