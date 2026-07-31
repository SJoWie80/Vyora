# Vyora Release Notes

This document combines the public release notes. VyoraXR and VyoraTV are beta software; features and compatibility may change between releases.

## 0.1.0-beta3

- Cleaned up downloaded update APKs after the installed version catches up.
- Hidden the downloaded-update action when the cached APK is already installed.
- Published matching Quest and Android TV beta3 APKs.

## 0.1.0-beta2

- Fixed Quest update installation after an APK download completes.
- Added the downloaded-update fallback to the Quest Settings page.
- Kept the update flow aligned between VyoraXR and VyoraTV.
- Published matching Quest and Android TV beta2 APKs.

## 0.1.0-beta1

- VyoraXR can now download and install updates directly from GitHub.
- VyoraTV and VyoraXR automatically use their matching update packages.
- Added support for beta release updates.
- Improved country detection for Quest and Android TV installations.
- Fixed app update installation support on Meta Quest.
- Fixed build reliability for Quest and Android TV release packages.

## 0.1.0-alpha21

- Added anonymous telemetry and crash reporting for VyoraXR and VyoraTV.
- Added a privacy setting to opt out of telemetry.
- Added private dashboard controls for viewing and clearing crash data.
- Improved country and device reporting for Quest and Android TV installations.
- Removed the temporary crash-test control from VyoraXR.
- Published matching Quest and Android TV alpha21 APKs.

## 0.1.0-alpha20

- Added native Bluetooth support for compatible [OSSM](https://ossm.tech/) machines in VyoraXR without requiring Intiface Central.
- Added a dedicated OSSM setup page and movable control window.
- Added manual speed, stroke, depth, pattern and sensation controls with precise `-` and `+` adjustment.
- Added safe positioning, persistent control settings and stopped-by-default connection behavior.
- Added direct OSSM funscript playback for tagged Stash scenes.
- Added persistent funscript speed, stroke and depth controls, initially defaulting to 25%.
- Added contextual OSSM controls to the immersive VR player panel.
- Improved funscript synchronization with faster timeline lookup, removal of obsolete Bluetooth commands and speed-limit handling.
- Improved actuator stopping when playback pauses, ends or exits.
- Published matching Quest and Android TV alpha20 APKs.

## 0.1.0-alpha19

- Added a visible funscript badge to Stash scene thumbnails and scene details in VyoraXR and VyoraTV.
- Added a brighter neon waveform badge with transparent background and stronger thumbnail contrast.
- Improved funscript detection by checking both the scene tag and the available heatmap URL.
- Published matching Quest and Android TV APKs in the GitHub release.

## 0.1.0-alpha18

- Improved Wheel of Passion layout spacing and vertical sizing on Android TV.
- Enlarged the position display area while keeping the controls visible.
- Fixed clipped status text such as `The wheel is spinning...`.
- Fixed clipped result names such as `Cowgirl`.
- Added consistent font padding and bottom spacing around the result controls.
- Published matching VyoraTV and VyoraXR APK assets in the GitHub release.

## 0.1.0-alpha17

- Added a dedicated Games destination to the VyoraTV sidebar between Online and saved sources.
- Added an offline Truth or Dare party game with 2-8 players and Warm, Spicy and Wild intensity choices.
- Added English, Dutch, German and French game prompts with per-player intensity selection and repeat protection.
- Added TV-remote navigation, Back handling and clear high-contrast focus states throughout the game flow.
- Improved game-card sizing, prompt readability, spacing and transparent artwork presentation.
- Refined Start, Next player and Quit focus feedback for better D-pad visibility.
- Updated public documentation with current privacy-redacted VyoraTV screenshots and Android TV sideload instructions.
- Replaced the framed VyoraXR README image with transparent Vyora XR/TV branding.

## 0.1.0-alpha16

- Redesigned VyoraTV around a modern two-panel library with dedicated Home and Online views.
- Added Home rows for recent Stash scenes and currently active live rooms.
- Improved source branding, media-card sizing and thumbnail aspect-ratio handling.
- Refined D-pad focus, Back navigation and focus restoration across scenes, actors, studios and galleries.
- Added and repaired pagination for Stash scenes and studios, including reliable thumbnail reloads between pages.
- Improved gallery navigation, photo selection, gallery titles and fullscreen image viewing.
- Moved online-source controls into Manage Sources and simplified the main Settings screen.
- Added GitHub update checking, downloading and installer handoff for VyoraTV; VyoraXR links to the release page.
- Updated release checks and public documentation for the renamed `SJoWie80/Vyora` repository.
- Made the VyoraTV player title bar hide and return together with the playback controls.
- Fixed vertical D-pad navigation so focus stays in the left sidebar through sources, local media, Settings and Quit.

## 0.1.0-alpha15

- Added Android TV screenshots to the public documentation with scene thumbnails anonymized.
- Improved TV D-pad navigation through scene, studio, actor, tag and gallery grids.
- Restored selected-tile focus after Back navigation and content reloads.
- Added compact loading feedback for TV scenes and directories.
- Improved TV dialog focus and keyboard behavior.
- Adjusted TV side-panel sizing so the center library keeps the available space.
- Improved Stash gallery title mapping when optional fields are empty.
- Added the Android TV launcher banner and VyoraTV branding.

## 0.1.0-alpha14

- Removed the retired Legacy Bridge source from the Quest and Android TV interface.
- Kept Stash Direct, PLAYA, local/LAN sources and Intiface Central available.
- Restored Quest-specific focus and native Oculus behavior after the Android TV split.
- Improved TV reconnect handling without repeatedly opening focus-stealing windows.
- Added capability-aware Intiface output for vibration and linear/position actuators.
- Added TV seek/intensity feedback overlays and accelerated D-pad seeking.
- Preserved the existing shared signing and local app data during release installation.

## 0.1.0-alpha13

- Added the VyoraTV Android TV edition with dedicated 2D library branding and layout.
- Added TV-focused D-pad navigation and consistent focus highlights.
- Added auto-hiding TV playback controls with seek support.
- Refined shared Meta Quest and TV source presentation.

## 0.1.0-alpha12

### Toy and funscript control

- Funscript actions are now sent to every connected Intiface device instead of only the selected device.
- Both actuators are addressed for each connected device.
- Stop commands are broadcast to all connected devices when playback ends, the scene changes or the connection is lost.
- Multi-device refresh and device-specific manual controls remain available.

### Stability

- Improved synchronization between the connected-device list and funscript playback.
- Preserved the existing Intiface reconnect, heartbeat and automatic scanning behavior.

## 0.1.0-alpha11

## 0.1.0-alpha11

### Highlights

- Added a complete English public user manual covering sources, Stash setup, VR detection, funscripts, player controls and troubleshooting.
- Improved Intiface Central connection monitoring with WebSocket heartbeat checks and automatic reconnect.
- The Intiface control popup now appears only after a successful connection and closes when the connection is lost.
- Connected toys and actuator counts refresh automatically while the control popup is open.
- Removed the placeholder Motor 1 control when no toy is connected.
- Added compact connected-toy names to the control interface.
- Funscript control now clearly uses an **Intensity** slider with a 50% default intensity.
- Improved stop handling so all supported actuators are stopped when playback ends or the connection is lost.

### Documentation and release packaging

- Clarified that VR mode is automatically detected from filenames and metadata; explicit tags are recommended for ambiguous files.
- Added official setup links for Stash, Intiface Central and Meta Quest developer setup.
- Combined the public alpha release history into this release-notes file.
- Public repository continues to contain release APKs and documentation only; application source code is not published.

## 0.1.0-alpha10

### Meta Store patch notes

- Improved VR controller handling for grip, trigger and B-button input.
- Kept VR zoom available through joystick up/down.
- Removed horizontal joystick movement for repositioning the VR image; repositioning is performed with grip.
- Improved player input handling and VR playback stability.

### Test note

This alpha contains an experimental change to Quest controller input during VR playback.

## 0.1.0-alpha9

### Highlights

- Added Stripchat as a separate live-cam source alongside Chaturbate.
- Added Stripchat Featured, Women, Men, Couples and Trans categories.
- Added Stripchat model thumbnails, viewer counts, search and pagination.
- Added direct Stripchat HLS playback for regular live streams.
- Removed the experimental Stripchat VR category because the public API does not expose a reliable separate SBS stream.
- Kept the regular Stripchat source available without making incorrect VR playback claims.
- Improved live-source separation and active-source highlighting in navigation.

### Notes

- Stripchat uses its public models endpoint with the configured source settings.
- The public endpoint reports VR capability but does not provide a separate SBS stream; VR is therefore not shown as a supported Stripchat mode in this release.
- Existing Stash, PLAYA VR, Chaturbate, Eporner, RedTube, ImageFap and local playback features remain available.

## 0.1.0-alpha8

This alpha adds local Stash scene favorites and improves the ImageFap gallery experience.

### What's new

- Added a star button to Stash scene details.
- Added a Favorites tab to the Stash navigation panel.
- Favorites are stored locally per user and per Stash server.
- Added ImageFap gallery photo counts below gallery titles.
- Fixed ImageFap category links and category loading.
- Added a compact Online Sources menu for Live Cams, RedTube, Eporner and ImageFap.

### Improvements

- ImageFap gallery cards now have enough height for title, thumbnails and photo count.
- ImageFap galleries load all available photo pages for accurate counts.
- Online Sources automatically collapses when switching to another source.
- Stash scene loading remains compatible with older Stash GraphQL schemas.

### Notes

- Stash favorites are local to the VyoraXR installation and are not written back to the Stash server.
- VyoraXR does not host media. Users configure and access their own compatible sources.

## 0.1.0-alpha7

This alpha expands online sources and improves navigation, gallery viewing and playback controls.

### What's new

- Added Eporner with search, sorting, VR discovery and pagination.
- Added RedTube as an optional source with native browsing and in-app playback.
- Added volume controls across the available players.
- Added fullscreen gallery viewing without the side panels.
- Added right-stick previous/next navigation while viewing gallery photos.

### Improvements

- Live Cams now refreshes when reopening a category.
- Back and B-button behavior is more consistent throughout the app.
- Gallery, scene and directory pages retain their page and scroll position more reliably.
- Portrait and landscape photos maximize available height without cropping.
- Improved thumbnail caching, retries and source switching.
- Added player and VR-exit stability fixes.

### Notes

- Eporner's official API currently exposes videos, but no supported photo-gallery endpoint.
- VyoraXR does not host media. Users configure and access their own compatible sources.
