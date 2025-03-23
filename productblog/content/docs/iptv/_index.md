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

[![image](/images/storeBadge.webp)](https://www.microsoft.com/store/productId/9PKMDLWBC8ZJ?cid=officialwebsite)

or use winget command `winget install 9PKMDLWBC8ZJ` in terminal -> Then enter `y`.

## Q&A Trouble shoot

### Instant crash after loading channels

Please install the graphic driver on the device. The app uses software decoder to play video.

### Video glitch during streaming

Switch playback engine in `Settings`.

### Unable to streaming video in background

Ditto. Switch to `System` playback engine in `Settings`.

### Random crash while switching between channels

Ditto again. `VLC` might crash if there is bad connection during the channel switch.

### Unable to parse the channel list

There are two circumstances:

- 1. The m3u/8 list does not follow the guideline. There is nothing we can do about this.

- 2. Our parsing logic is unable to parse the list. Please send the list to us via mail if it's convenient for you.

### Default system players does not load user agent required channel

Currently only other two video engines support user agent required channel. Please change video playback engine in settings if you wish to play channels like this.

### Is there mobile version for IPTV Fluent

iOS version is under development. Though there is no release date for it yet, it'll be up once it's ready.
