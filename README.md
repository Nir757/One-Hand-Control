# One Hand Control Releases

This repository is **release-only** and does not include source code.

## Privacy

- One Hand Control does not collect, store, or transmit personal data.
- Gesture settings and app preferences remain on your device.

## Download and Install (Release Repo)

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

## Notes

- Source code is maintained in a separate private repository.
- Use Issues for bug reports and release feedback.

---

## Project README (Mirrored)

# One Hand Control

One Hand Control is an Android app that uses an `AccessibilityService` overlay to trigger actions from configurable edge gestures. It is designed for one-handed navigation and quick system controls without reaching hardware or nav buttons.

## Privacy

- One Hand Control does not collect, store, or transmit personal data.
- Gesture settings and app preferences remain on your device.

## Download and Install (Recommended)

1. Open the latest GitHub release and download `One-Hand-Control.apk`.
2. Install using one of these supported methods:
   - **Package installer flow (phone):** open the APK, allow **Install unknown apps** when prompted, and confirm install.
   - **ADB flow (computer):** `adb install -r One-Hand-Control.apk`.
3. Launch One Hand Control.
4. Enable the accessibility service for One Hand Control in Android settings.
5. Grant System Settings permission only if you use brightness, auto-rotate, or blackout actions.

## Highlights

- Configurable edge zones on left, right, top, and bottom sides
- Gesture-to-action mapping per zone (tap, swipe, long press, swipe+hold, pull+slide, and more)
- Split-zone support for side edges
- Optional visual edge indicators, haptic feedback, and auto-hide behavior
- Macro recording and playback for app-specific interaction sequences

## Project Structure

- `app/src/main/java/com/onehandcontrol/app/ui` - Compose-based settings and configuration screens
- `app/src/main/java/com/onehandcontrol/app/service` - Edge gesture accessibility service and overlays
- `app/src/main/java/com/onehandcontrol/app/action` - Gesture action models and execution layer
- `app/src/main/java/com/onehandcontrol/app/data` - Preferences, edge-zone configs, macro data models

## Project Context

- `docs/project-state.md` - current architecture, dependencies, permissions, and goals
- `docs/context-workflow.md` - documentation workflow rules for feature and bug-fix sessions
- `docs/dev-log.md` and `docs/bug-fixes.md` - reviewed history for completed work
- `docs/android-app-context.md` - Android-specific implementation context

## Requirements

- Android Studio (latest stable recommended)
- Android SDK with minimum API 26
- JDK 17+
- A connected device/emulator for install and runtime testing

## Build and Install

```powershell
# Build and install debug APK to connected device
./gradlew installDebug

# Build release APK (falls back to debug signing if release secrets are not set)
./gradlew assembleRelease
```

Release output:

- `app/build/outputs/apk/release/One-Hand-Control.apk`

### Release Signing (Do Not Commit Secrets)

For real GitHub release APKs, provide release signing secrets through environment variables
or Gradle properties:

- `RELEASE_STORE_FILE`
- `RELEASE_STORE_PASSWORD`
- `RELEASE_KEY_ALIAS`
- `RELEASE_KEY_PASSWORD`

Keep the keystore file and all signing values out of git. This project ignores common key
file extensions and `local.properties` by default.

## Required Permissions

One Hand Control depends on runtime/system permissions:

- Accessibility service (`BIND_ACCESSIBILITY_SERVICE`) to run the gesture overlays
- Settings write permission (`WRITE_SETTINGS`) for brightness, auto-rotate, and blackout-style actions
- Normal app permissions for vibration and audio settings
- Manifest package-visibility queries for launcher and shortcut picking

## Running the App

1. Install the app from GitHub Releases (recommended), or build with `./gradlew installDebug`
2. Open One Hand Control settings
3. Enable the accessibility service in system settings
4. Grant System Settings permission if your mapped actions need it
5. Configure each edge zone and map gestures to actions

## Size and Position

- Open an edge, then use **Size & Position** to adjust thickness, length, and offset.
- For left/right split edges, scroll down in the Size & Position screen to access **Zone 2** adjustments.

## Notes

- Gesture behavior and available actions vary by Android version and OEM restrictions.
- Some advanced actions may require additional permission grants from Android settings.
