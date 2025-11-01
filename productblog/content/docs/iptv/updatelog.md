---
title: Update log
weight: 4
linkTitle: Update Log
prev: /docs/iptv/iptvplus
---

IPTV Fluent is constantly receiving updates and in active development right now.

## v1.0.44

Release date: TBD

- Feature: Debugger for failing to grab a list or play a channel

## v1.0.43

Release date: 2025/11/15

- Improvement: Improve pinned speed for the first time under Win 11
- Improvement: Some UI adjustment
- Bug fixes: Fix the failure of downloading list from some short url sites like shortio, etc
- Bug fixes: Fix the failure of downloading EPG when the EPG is a huge list
- Bug fixes: Fix the top right color not changing while auto theme switched

## v1.0.42

Release date: 2025/10/24

- Improvement: Provide higher-resolution icons
- Improvement: On the EPG page, quickly navigate to a specific page by tapping the number
- Improvement: (FFMPEG|System Engine) Take a snapshot by right-clicking
- Bug fixes: (PC) Fix an issue where failing to navigate or playing a channel after clicking a pinned tile while the app was open
- Bug fixes: (PC) Fix an issue where some channels could not be pinned to Start
- Bug fixes: (Console) Remove the language options in settings that do not match the system

## v1.0.41

Release date: 2025/9/25

- Feature: Cache management for checking and clear temp files
- Improvement: Online list in library gets new vertical view switch
- Improvement: Add header in narrow state window for better readability
- Bug fixes: (VLC) Inaccurate progress slider's position under some circummenstances
- Bug fixes: (VLC) Volume changing doesn't work while video paused

## v1.0.40

Release date: 2025/8/27

- Pro Feature: (PC|VLC|Beta) Recording video and save into video file | Free during beta
- Pro Feature: Force refresh for missing channels in `COG` icon
- Feature: (VLC|FFMPEG) Customize Playback options in order to add referrer, user-agent, etc
- Feature: (Beta) Play seek support for older programmes (Server is required to support old programmes | Channels have to be added into favorite)
- Improvement: Testing new Undo button when unlike channel accidentally
- Improvement: (VLC) Adjust some icons to represent the features more accurately and native
- Improvement: UX with some items with horizontal scroll actions

## v1.0.39

Release date: 2025/8/4

- Pro Feature: (PC|Beta) Play a channel in new Window
- Improvement: Cache in local for FTP server by right clicking file
- Improvement: Minor UI tweaks
- Bug fixes: Display correct channel name while using remote control for dialing numbers
- Bug fixes: Fix some circumstances which unable to play videos in ftp server

## v1.0.38

Release date: 2025/7/14

- Feature: (PC) New `Remote Control` option in Settings to enable remote control or air mouse navigation
- Pro Feature: Open channels with the system media player or VLC UWP — right-click a channel in the Channels page
- Improvement: Set preferred subtitle track for VOD playback
- Improvement: Improved translations in some languages
- Bug fixes: Corrected time offset for channels on the EPG page
- Pro Feature: Option to force server-side transcoding for Jellyfin and Emby
- Bug fixes: Fixed black poster images in poster view for Jellyfin and Emby
- Bug fixes: Fixed incorrect episode order for Jellyfin and Emby

## v1.0.37

Release date: 2025/7/1

- Feature: New fullscreen big picture mode available in settings
- Pro Feature: Poster wall modification for Jellyfin and Emby
- Feature: Search in Poster wall for Jellyfin and Emby
- Feature: Cross platform resume play in Poster wall for Jellyfin and Emby
- Feature: Genre view for Jellyfin and Emby
- Feature: Unplayed mark in poster view, mark videos played and favorited for Jellyfin and Emby
- Improvement: Enhanced fullscreen touch device control and navigation
- Improvement: Better gamepad control on PC
- Improvement: Launche menu includes `Media hub` available for all users
- Bug fixes: Episodes order correction in Series Page for Jellyfin and Emby
- Bug fixes: Unusual occassion entering an episode detail after crashing for Jellyfin and Emby
- Bug fixes: Typo fix

## v1.0.36

Release date: 2025/6/22

- Feature: Support complete Jellyfin or Emby's poster wall with genre types
- Improvement: Some typo fixes
- Major Bug fixes: Fix some XC M3U lists won't be downloaded

## v1.0.35

Release date: 2025/6/19

- Feature: (Console) Support 4K HEVC Codec video on Emby or Jellyfin server by using server transcoding
- Pro Feature: (Beta) Movie/TV wall view for Jellyfin and Emby media servers
- Pro Feature: (PC) Quick guide for system video codec downloads
- Pro Feature: (PC) Pin media server to start menu
- Improvement: More native Turkish translation special thanks to community numbers!
- Bug fixes: Hide the language in settings which is not supported by the system

## v1.0.34

Release date: 2025/6/8

- Feature: (Beta) New media hub for Jellyfin, Emby and FTP as media servers
- Feature: (Beta) Enable auto scan Jellyfin or WebDAV media server in local network
- Feature: (Beta) Auto load external subtitles in Jellyfin or Emby media server
- Feature: Add disable tap to pause preventing from accidentally pause the stream or video
- Improvement: (PC) New keyboard shortcuts including (Ctrl+T)theatre mode, (Ctrl-←)quick rewind, (Ctrl+→)fast forward, (Ctrl+I)video info
- Improvement: (VLC) Relocate subtitle and audio track selector for better UX
- Improvement: (VLC) improve video control panel
- Bug fixes: Fix some issues with loading big list in local M3U files
- Bug fixes: (FFMPEG) Fix subtitles  stack together once added new subtitle
- Bug fixes: (VLC) Fix unable to load multiple external subtitles
- Bug fixes: (VLC | PC) Fix the progression lost for VOD when get back to the playing page
- Bug fixes: (Console) Fix the app locked in the fullscreen after navigating away from the playing page

## v1.0.33

Release date: 2025/5/29

- Pro Feature: (Beta) New media hub for DLNA, WebDAV and local as media servers
- Pro Improvement: Autofill EPG URL under XC if there is no EPG set before
- Improvement: Add restore `lifetime` purchase button

## v1.0.32

Release date: 2025/5/19

- Pro Feature: Add new `every month` option for update frequency
- Feature: Share encrypted channel with expiration date (App install required by other people)
- Improvement: Auto complete incomplete URL for XCodes
- Improvement: Improve the parser for M3U lists
- Improvement: Typo fixes

## v1.0.31

Release date: 2025/5/1

- Bug fixes: Fix some lists failed to load channels

## v1.0.29

Release date: 2025/4/16

- Feature: (VLC) Change video scale
- Feature: (VLC) Change audio delay
- Feature: (VLC) Allow controls dock at the bottom in experimental feature
- Improvement: UI improvements in Media Servers folder
- Improvement: (Console) Optimization for TV overscan & remove blank border while fullscreen
- Improvement: (Console) Add FFmpeg playback engine in Settings
- Improvement: (Console) Add Stalker Portal list support
- Bug fixes: Fix mouse hidden even side menu is open while fullscreen
- Bug fixes: Keep lowering the crash possibilities in VLC playback engine

## v1.0.28

Release date: 2025/3/24

- Bug fixes(Major fix): Lower the crash posibility in VLC playback engine
- Bug fixes: Lower the UI freezes after switching to unreponsive channels
- Experimental feature: VLC add force fresh video option
- Improvement: Mark EPG's date in the blade guide

## v1.0.27

Release date: 2025/2/20

- Pro Feature: VLC add OLED screen burn-in preventor
- Feature: VLC add custom video ratio option
- Feature: VLC add subtitle delay option
- Improvement: Enhanced loved list management
- Improvement: Love channel while playing
- Improvement: Edit the online list
- Bug fixes: Certain EPG url unable to switch between pages
- Bug fixes: Loading indicator for changing audio ouput device

## v1.0.26

Release date: 2025/1/20

- Feature: VLC add custom speed options
- Feature: Pin channel or list to start menu for quick launching
- Improvement: Add title tooltip for the blade channel menu
- Improvement: Some UE adjustment
- Bug fixes: Fix some mis-translation in Italian special thanks to Alessandro
- Bug fixes: Fix blank genre which might cause crash
- Bug fixes: Fix unable to purchase life-time plus if the app is under subscription

## v1.0.25

Release date: 2024/11/8

- Feature: Change default online list in `Settings`
- Bug fixes: Show title on Live Tile under Win10  

## v1.0.24

Release date: 2024/10/28

- Feature: Pro user can play local videos
- Feature: Pro user can play media servers videos
- Bug fixes: Update VLC playback engine core to lower the crash

## v1.0.23

Release date: 2024/9/10

- Feature: Support channels which requires user-agent or referrer
- Bug fixes: Improve channel list parse

## v1.0.22

Release date: 2024/8/30

- Pro Feature: Export multi-selected channels to m3u list locally
- Feature: Edit channel in local list
- Adjustment: Better experience when add a channel to local list
- Adjustment: Minor UI adjustment in EPG page

## v1.0.21

Release date: 2024/8/19

- Pro Feature: Add custom auto sleep time in settings
- Feature: Add `Stalker Portal` (beta) online list support
- Feature: Add reorder channel in favorite and local list
- Bug fixes: Fix some navigation loop

## v1.0.20

Release date: 2024/8/9

- Feature: More language support

## v1.0.19

Release date: 2024/8/2

- Bug fixes: Fix unable to switch channel under VLC player engine

## v1.0.18

Release date: 2024/8/2

- Feature: Cache online list
- Feature: New language support

## v1.0.17

Release date: 2024/7/29

- Feature: Add FFmpeg as video engine
- Feature: Add Background audio play using native engine
- Bug fixes: Fix some video playback issue using native engine
- Bug fixes: UI fixes under small window

## v1.0.16

Release date: 2024/7/26

- Feature: Add Xtream Codes parser
- Feature: Add txt file parse
- Feature: Change default list/grid
- Bug fixes: Blade bar ui fix
- Bug fixes: Fix some circumstances which stuck in fullscreen
- Bug fixes: Fix some circumstances which unable to enter compact mode under some channels

## v1.0.15

Release date: 2024/7/22

- Pro Feature: Stand alone EPG page
- Feature: New video info in blade bar
- Feature: Change stream video track
- Feature: Change stream audio track
- Feature: Change stream subtitle
- Feature: Option to enable hardware decoding
- Bug fixes: EPG list for different time zones
- Bug fixes: Video restart after pausing and replaying the VOD

## v1.0.14

Release date: 2024/7/17

- Feature: New 'LIVE' icon in video page
- Feature: New blade right bar in video page
- Feature: Redeigned EPG list UI in video page
- Feature: New time finder for VOD in video page
- Feature: Grid list in channels page with icon
- Feature: New library page
- Feature: Rename saved online list in library page
- Feature: Reorder saved online list in library page
- Feature: UI tweaks in Settings page
- Bug fixes: Switch to online list when refreshes in channels page