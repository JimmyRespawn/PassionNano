---
title: "Configurations"
weight: 2
prev: /docs/iptv/get-started
next: /docs/iptv/iptvplus
---

Though IPTV Fluent is ready to play streaming as long as you have personal IPTV Provider, but still it offers powerful customization settings.

<!--more-->
## Menu layout

To adjust settings in IPTV Fluent, simply click `Settings` button on the left menu.

{{< filetree/container >}}
  {{< filetree/folder name="IPTV Fluent" state="open">}}
      {{< filetree/file name="Live TV" >}}
      {{< filetree/file name="Channels" >}}
      {{< filetree/file name="Library" >}}
      {{< filetree/file name="Settings" >}}
  {{< /filetree/folder >}}
{{< /filetree/container >}}

## General settings

### Launch menu

![image](https://od.lk/s/200607426_u0Sx5/launchmenu.png)

There are `Live TV`, `Channels` and `Library`. After launching the app, it'll immediately open the option you choose.

### App language

![image](https://od.lk/s/200607851_yegn7/language.png)
There are 20 language options in the app.

Except English, French, Spanish and Chinese, other language is translated by AI and machine. Join the translation group to help us translating the app.

If your OS does not have the language pack, the app language won't take effect after changing.

## Playlist sync

![image](https://od.lk/s/200608026_n1oNA/sync.png)

Online playlist and favorite list added by users can be synced between devices like desktop and tablet via OneDrive.

You have to manually click upload and download between devices. Auto sync is under development.

Currently this feature is only available for IPTV Plus.

## Playback settings

### Playback engine

![image](https://od.lk/s/200609031_t4bhu/playbackengine.png)

Playback engine is the core player behind streaming. If you encounter any issue while playing some live stream, you may change the playback engine.

1: VLC has better graphics and source playbility support.

2: Native system player has better RAM memory usage management and stability management.

3: FFMpeg has better stream support but consume more RAM memory usage.

### Electronic programme guide

![image](https://od.lk/s/200611282_LCp8I/EPG.png)

Custom epg required a external xml link which may be provided by your IPTV Provider or you may search it online.

![image](https://od.lk/s/200612577_CWt9Q/epg2.png)
It will display upcoming programmes after url has been setted.

### Auto sleep

![image](https://od.lk/s/200612991_jD6Gx/autosleep.png)
App supports auto shut down after certain amount time.

## List settings

### Default list view

In channel list, default it displayed as single line list.

There is an `Grid` option to show it with programme logo.

### Auto detect latency

There may be some situations which you retrieve unreliable m3u list online.

Many of the channels within it may be unavailable in your region.

Turn on this feature will auto hide those channels after loading the online list.

### Update frequency

`Every day`, `Every month` option enables cache the online list every day or every month without loading the list every time.

## Read More

- [Wiki: Electronic program guide](https://en.wikipedia.org/wiki/Electronic_program_guide)