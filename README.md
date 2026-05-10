# One Hand Control Releases

This repository is **release-only** and does not include source code.
The app would soon be featured in the play store, you can send me an email to join the testing group. 
nir757.appsupport@gmail.com

## Privacy

- One Hand Control does not collect, store, or transmit personal data.
- Gesture settings and app preferences remain on your device.

## Download and Install

1. Open the [Releases](https://github.com/Nir757/One-Hand-Control/releases) page.
2. Download the latest APK asset.
3. Install using one of these supported methods:
   - **Package installer flow (phone):**
     - Open the APK on your device.
     - If blocked, enable **Install unknown apps** for the app you used to open the APK (browser/files), then retry.
     - Confirm the install prompt.
   - **ADB flow (computer):**
     - Enable Developer options and USB debugging on the phone.
     - Connect the phone and run:
       - `adb install -r One-Hand-Control.apk`
4. Launch One Hand Control.
5. Enable the accessibility service for One Hand Control in Android settings.
6. Grant System Settings permission only if you use brightness, auto-rotate, or blackout actions.

## App Overview

One Hand Control is an Android app that uses an `AccessibilityService` overlay to trigger actions from configurable edge gestures. It is designed for one-handed navigation and quick system controls without reaching hardware or nav buttons.

## Highlights

- Configurable edge zones on left, right, top, and bottom sides
- Gesture-to-action mapping per zone (tap, swipe, long press, swipe+hold, pull+slide, and more)
- Split-zone support for side edges
- Optional visual edge indicators, haptic feedback, and auto-hide behavior
- Macro recording and playback for app-specific interaction sequences

## Requirements

- Android Studio (latest stable recommended)
- Android SDK with minimum API 26
- JDK 17+
- A connected device/emulator for install and runtime testing

## Required Permissions

One Hand Control depends on runtime/system permissions:

- Accessibility service (`BIND_ACCESSIBILITY_SERVICE`) to run the gesture overlays
- Settings write permission (`WRITE_SETTINGS`) for brightness, auto-rotate, and blackout-style actions
- Normal app permissions for vibration and audio settings
- Manifest package-visibility queries for launcher and shortcut picking

## Running the App

1. Install the app from GitHub Releases (recommended).
2. Open One Hand Control settings.
3. Enable the accessibility service in system settings.
4. Grant System Settings permission if your mapped actions need it.
5. Configure each edge zone and map gestures to actions.

## Notes

- Source code is maintained in a separate private repository.
- Use Issues for bug reports and release feedback.
