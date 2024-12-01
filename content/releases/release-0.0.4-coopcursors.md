+++
author = "Alexis Rosovsky"
title = "0.0.4"
date = "2024-12-01"
description = "Version 0.0.4"
tags = [
    "release",
]
categories = [
    "release",
]
+++

New version 0.0.4 of CoopCursors is out !

## Links

* [Windows MSI installer](https://storage.googleapis.com/coopcursors/windows/msi/CoopCursors-0.0.4.msi)
* [Linux JAR Server](https://storage.googleapis.com/coopcursors/linux/uberJar/CoopCursors-server-0.0.4-linux-amd64.jar)

## Jar links

Just in case, if there's a packaging issue for desktop builds.

* [Windows](https://storage.googleapis.com/coopcursors/windows/uberJar/CoopCursors-windows-x64-1.0.0.jar)


## Changes from previous version 0.0.3 (commit titles)

- Disable clickThrough when sending clicks to sink
- Initialize currentOperatingSystem only once
- Disable sending clicks state when overlay hidden
- Some package movement
- Use enum for right/left buttons
- Right click == 2 x)
- Server relay clicks
- Draw ClickCursor only for local peer
- Prevent silent exceptions in WSClient
- Send/Receive clicks
- Introduce ClickCursor and shortcut
- ClickMaker uses array for SendInput
- Remove fake election delays
- Promote/Demote sink feature
- Bump JNA versions
- Initial ClickMaker
- tmp
- Introduce coturn-shutdown cloud function
- Use relative coordinate over the network
- Don't send cursor position when cursor not in overlay
- Create overlay according to primary display dimensions
- Fix AccessToken duration
- Aborted embryo of Linux support
- Initial coturn setup

