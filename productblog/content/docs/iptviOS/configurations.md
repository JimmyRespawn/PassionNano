---
title: "Configurations"
weight: 2
prev: /docs/iptvos/get-started
next: /docs/iptvos/iptvplus
hide_navbar: true
hide_edit: true
---

Though IPTV Fluent is ready to play streaming as long as you have personal IPTV Provider, but still it offers powerful customization settings.

<!--more-->
## 1. Menu layout

To adjust settings in IPTV Fluent, simply click `Settings` button at the tab menu.

{{< filetree/container >}}
  {{< filetree/folder name="IPTV Fluent" state="open">}}
      {{< filetree/file name="Channels" >}}
      {{< filetree/file name="Library" >}}
      {{< filetree/file name="Settings" >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

## 2. List settings

### 2.1 Auto detect latency

There may be some situations which some videos in the server has unreliable internet connect.

Turn on this feature will auto detect those channels' latency after loading the online list.

### 2.2 Update frequency

`Every day` and `Every month` options enable cache the online list every day or month without loading the list every time.

## 3. Playback settings

### 3.1 Playback engine

Playback engine is the core player behind streaming. If you encounter any issue while playing some live stream, you may change the playback engine.

1: VLCKit has better graphics and source playbility support.

2: Native system player has better RAM memory usage management, stability management and PIP feature.

### 3.2 Cellular Warning

If the device is under cellular network. The video streaming might cost a handful data plan. It'll warn you if you open a video under the circumstances.

Be aware, it will not warn you while playing video.

## 4. General settings

### 4.2 Launch menu

There are `Channels` and `Library`. After launching the app, it'll immediately open the option you choose.

### 4.3 Language

There are 2 language options in the app. English and Chinese Traditional.

Join the [Crowdin translation group](https://crowdin.com/project/iptvfluentswift) to help us translating the app.
