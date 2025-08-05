---
linkTitle: IPTV
title: IPTV Fluent
prev: /docs/
next: /docs/iptv/get-started
---

## Introduction

IPTV Fluent is a powerful software solution designed for seamless IPTV streaming and management.

This section covers tutorial how to use IPTV Fluent.

<!--more-->

{{< cards >}}
  {{< card link="get-started" title="Get-Started" icon="template" >}}
  {{< card link="configurations" title="Configurations" icon="adjustments" >}}
  {{< card link="iptvplus" title="What's in IPTV Plus" icon="sparkles" >}}
  {{< card link="updatelog" title="Update log" icon="sparkles" >}}
{{< /cards >}}

### How to use?

Simply type any m3u links you found online into [Search channels m3u/8 link] on the left and press _Enter_.
![VLC Network Panel](https://github.com/JimmyRespawn/IPTV-Fluent/raw/main/doc/images/SearchSectionIPTVFluent.png?raw=true)

### Where can I find m3u link?

Type 'iptv' into github search section.
Or type 'm3u links' on any search engine.

### Terms of Service

IPTV Fluent does not host or distribute any content or re-direct you to any reseller. Please find m3u8 or m3u link provided by other legal IPTV providers.

### Download Link

Windows & Xbox version:

[![image](/images/storeBadge.webp)](https://www.microsoft.com/store/productId/9PKMDLWBC8ZJ?cid=officialwebsite)

or use winget command `winget install 9PKMDLWBC8ZJ` in terminal -> Then enter `y`.

iOS & iPad version：

[![image](https://od.lk/s/221204631_BUHm4/AppStoreDownloadBadge.png#left)](https://apps.apple.com/app/id6744343679?pt=127753526&mt=8&ct=officialwebsite&platform=iphone)

or scan QR code to download for free:

<img src="/images/IPTVFluentAppStoreQRCode.webp" width="260" alt="QRCode" />

## Q&A Trouble shoot

### Instant crash after loading channels

Please install the graphic driver on the device. The app uses software decoder and hardware decoder to play video.

### Unable to streaming video in background

You may exit the playing page to library page in order to release the video comsumption, then direct the app to the background.

### Video glitch during streaming

Switch playback engine in `Settings`.

### Random crash while switching between channels

Ditto. `VLC` might crash if there is bad connection during the channel switch.

### Unable to parse the channel list

There are two circumstances:

- 1.The M3U/8 list does not follow the guideline. There is nothing we can do about this.

- 2.Our parsing logic is unable to parse the list. Please send the list to us via mail if it's convenient for you.

### Default system players does not load user agent required channel

Currently only other two video engines support user agent required channel. Please change video playback engine in settings if you wish to play channels like this.

### Is there mobile version for IPTV Fluent

iOS and iPad verison is available at app store. [Click here to download for free](https://apps.apple.com/app/id6744343679?pt=127753526&mt=8&ct=officialwebsite&platform=iphone).

### Media Hub for Emby, Jellyfin and WebDAV

Starting at v1.0.34 for Windows & Xbox version. The app supports Emby, Jellyfin, WebDAV and DLNA as media servers.

Access it by clicking the top right botton in the `Library` Page.

The media info is accessible for Emby and Jellyfin servers. Currently there is no modification for poster wall yet. We'll see how it performs as media player now.

The app is aiming to be a multi-media hub as Infuse and Kodi did in iOS and Android.

P.S. On console the app is using server transcoding for 4K HEVC videos due to codec issue. Other videos are using the native hardware decode.

### How to launch on startup or pin it to desktop

Follow this instruction: [Tutorial here](/blog/iptvfluentlaunchonstartup/).
