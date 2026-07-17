<p align="center">
  <img alt="Files hero image" src="./fastlane/metadata/android/en-US/images/featureGraphic.png" />
</p>

<p align="center">
  <a style="text-decoration:none" href="https://github.com/Fodi9159/Sefirah-Android/releases/latest"><img src="https://img.shields.io/github/v/release/Fodi9159/Sefirah-Android?label=patched%20release&logo=github" alt="Latest Patched Release" /></a>
  <a style="text-decoration:none" href="https://github.com/shrimqy/Sefirah-Android"><img src="https://img.shields.io/badge/source-shrimqy/Sefirah--Android-blue?logo=github" alt="Upstream Source" /></a>
</p>

# Sefirah Android — Patched Fork

This is a **patched fork** of [shrimqy/Sefirah-Android](https://github.com/shrimqy/Sefirah-Android). It automatically tracks upstream releases and applies modifications on top.

## 🔧 Patches Applied

| Patch | Description |
|---|---|
| **Clipboard Quick Settings Tile** | Added `TOGGLEABLE_TILE` meta-data to `ClipboardTileService` so the clipboard-push tile appears in the quick settings editor and can be added as a one-tap tile (instead of using the notification) |

## 📦 Releases

Every day (or on demand), the [sync workflow](.github/workflows/sync-and-build.yml) checks the upstream repo for new releases. When found:

1. Fetches the upstream source
2. Applies patches
3. Builds the debug APK
4. Publishes it as a release tagged `vX.Y.Z-patched`

➡️ **[Download the latest APK](https://github.com/Fodi9159/Sefirah-Android/releases/latest)**

> ⚠️ **Debug build** — signed with a different key than the Play Store version. Uninstall the official app first before installing.

## 📖 Original README (from upstream)

**Sefirah** is an opinionated phone link alternative designed to enhance your workflow with seamless clipboard and notification sharing between your Windows PC and Android device.

### Features

- **Clipboard Sharing**: Seamlessly share clipboard content between your Android device and Windows PC.
- **Media Control**: Control media playback and volume of your PC from android.
- **File Sharing**: Share files between your devices easily.
- **Storage Integration**: Integrate your Android storage into the Windows Explorer.
- **Notification**: Allows toasting the notifications from your android in desktop.
- **Screen mirroring**: Mirror and control the Android device via scrcpy.

### Limitations

- Due to Android's restrictions, sensitive notifications are no longer visible from Android 15 onwards.
- To work around this limitation, grant the permission via ADB: `adb shell appops set com.castle.sefirah RECEIVE_SENSITIVE_NOTIFICATIONS allow`

### Installation

| Platform | Link |
|---|---|
| **Windows** | [Microsoft Store](https://apps.microsoft.com/detail/9PJV6D1JPG0H) |
| **Android** | [Google Play](https://play.google.com/store/apps/details?id=com.castle.sefirah) / [IzzyOnDroid](https://apt.izzysoft.de/fdroid/index/apk/com.castle.sefirah) |
