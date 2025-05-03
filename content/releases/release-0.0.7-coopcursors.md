+++
author = "Alexis Rosovsky"
title = "0.0.7"
date = "2025-05-03"
description = "Version 0.0.7"
tags = [
    "release",
]
categories = [
    "release",
]
+++

New version 0.0.7 of CoopCursors is out !

## Links

* [Windows MSI installer](https://storage.googleapis.com/coopcursors/windows/msi/CoopCursors-0.0.7.msi)
* [Linux JAR Server](https://storage.googleapis.com/coopcursors/linux/uberJar/CoopCursors-server-0.0.7-linux-amd64.jar)

## Jar links

Just in case, if there's a packaging issue for desktop builds.

* [Windows](https://storage.googleapis.com/coopcursors/windows/uberJar/CoopCursors-windows-x64-1.0.0.jar)


## Changes from previous version 0.0.6 (commit titles)

- Switch to GCS since awscli is broken with GCS interop
- Replace testaws by testgcs
- Try windows 2019
- Use windows-2022 runner
- Force install working aws-cli version
- Log aws version
- Add test in testaws workflow
- Fix typo in testaws workflow
- Disable build of old WS LAN only server in release workflow
- Update workflow deploying rooms-function
- Move servers related module to servers directory
- Moved tools module to tools directory
- Fix cryptotool build
- Moved libselfupdater in features module directory
- Sink should notify newcoming peers it is Sink
- Logging adjustments
- Don't lose sink when a non sink user disconnects
- Reformated webrtcmeshcontroller
- Have aider start in chat mode
- Cleanup a bit after aider
- feat: Poll DataChannel state to reliably signal OPEN, handle CONNECTING
- feat: Signal data channel open and send initial peer state
- refactor: Improve WebRTC mesh connection management and cleanup
- refactor: Simplify peer management with reactive state flows
- feat: Expose peer connection states as a state flow
- Debug receivedPeers meshcontroller
- feat: Add peers to receivedPeers as they appear in manager state
- feat: Update receivedPeers on peer connection state changes
- Fix serialization issue due to missing build plugin
- Fix connection initiation
- fix: Remove unused variable currentPeerIds in peer state watcher
- Add peer to manager when peerconnection created
- Fix room function imports
- Various aider invocation params
- WIP new webrtc integration into composeApp
- Move new shared deps to commonMain deps
- SignalingClient implements SignalingClientInterface
- WIP Start webrtc integration in composeApp
- Introduced webrtc-coopcursors-shared for DataChannelMessages
- InputSharedDesktop -> InputShared since not desktop specific
- Integration test webrtc-mesh-desktop
- refactor: Use logging utility in mesh integration tests
- test: Limit dispatcher parallelism in integration test
- chore: Replace println with Log utility
- fix: Initialize peer connection observer before use
- fix: Fix manager state transitions on signaling state changes
- test: Add integration test for mesh manager peer connection & data channel
- WIP refactor webrtc
- remove misplaced webrtc-mesh-desktop module (misconfigured aider)
- Remove old LAN-only (pre-webrtc) websocket server
- tmp aider.sh
- refactor: Remove duplicate TestSignalingClient definition
- test: Add test implementation for SignalingClientInterface
- test: Add test signaling client
- Have aider.sh use whole diff for now
- Raw AI implem of webrtc-mesh-desktop
- WIP webrtc rework
- feat: introduce isolated WebRTC mesh management module
- aider script for gemini options
- Fix MouseButton package
- Fix ClickMaker package
- Prepare webrtc module
- Minor comment build.gradle
- Move SignalingClient in a dedicated feature module
- Moved FeatureState to shared module
- Fix input refactoring
- refactor: Move input-related code to new feature modules
- feat: Add feature modules and remove old dependencies in Gradle files
- Update composeApp with isolated features (config/platforms)
- refactor: Decouple ConfigManager from concrete Config class using generics
- feat: Implement ConfigManager for desktop configuration
- Isolate Platforms detection as a separate feature
- Desktop logging as a module
- Fix click generation
- Add aider files to gitignore
- feat: Add function to get virtual desktop dimensions on Windows.
- feat: Make clickAt use targetDisplayRect for coordinates
- Remove old WSClientController
- Update webrtc-java 0.10.0
- Workflow to deploy signalisation function
- WIP native testing
- remove hardcoded jdk
- Moved to webrtc package
- Remove DatachannelBuffers allocation for now
- UI for RoomUUID
- Fix ClickEvent coordinates handling
- Display local feedback when sending clicks
- Fix cursorPosition sending when overlay opened before connection
- Use channel instead of flow for ClickEvent
- Implement ClickMessage reception
- Don't send IceCandidate too early
- Display delay between received CursorPosition
- VERBOSE is a MutableStateFlow
- CursorPosition over webrtc
- Promote/Demote sink over webrtc
- Signaling: Silence unecessary exception
- Keep only logs from n previous launches
- Use version catalog for all libs
- Webrtc dependency according to currentOS
- Display RTT with RemotePeers
- Proper reconnection/disconnection with Webrtc
- Signaling: Don't use ConcurrentMap for clientContext
- Signaling: Don't drop messages upon client disconnection
- Begin transition to webrtc using p2pclientcontroller
- WebRTC ping with hardcoded roomUuuid. No UI yet.
- Move webrtc package to data
- Introduce P2PeersClient to manage P2P WebRTC connections
- Signal server out of WebRTCClient
- Rewrite signalisation server with Firestore
- Broke signaling pub/sub. Too slow.
- GraalVM native image for room-function, not functional yet
- Ktor Server switch from Netty to CIO
- Signaling and reconnection behavior improvements
- Crash when establishing DataChannel
- Introduce MyWebRTCClient
- Reworked PubSub Websocket bridge
- Setup for Pub/Sub as WebRTC signaling
- rooms-function depends on :shared
- Update deploy.md
- Commit coturn-shutdown module
- Coturn Starter uses SSE
- Add Rooms function bridging to Pub/Sub
- Revert "Switch to sharedflow for PeerContext.cursorFlow"
- Switch to sharedflow for PeerContext.cursorFlow
- Log unexpected -1,-1 cursor positions
- Log failed emit in flows
- Fix ClickSending using collectAsState
- Reduce delay stop cursor emit 300 -> 200ms
- Optionnally logs delay between received Cursor positions
- Managing Click events move to OverlayController
- Switch to ktor-cio
- Optimize overlay rendering for fast updates
- Fix MouseClickedEvent coordinates

