# Chrome VM Android 🌐

Chrome Android Mod with **Extension Support** and **Violentmonkey** Pre-installed.

## Mod Features

| Feature | Details |
|---------|---------|
| ✅ Extension Support | Patched `extensions.disabled` flag in native code |
| ✅ Violentmonkey Pre-installed | v2.36.0 bundled in assets |
| ✅ Package Changed | `com.android.chrome` → `com.android.chrome.vm` |
| ✅ App Name Changed | `Chrome` → `Chr-VM` |
| ✅ Full Signed | V2 + V3 APK Signature Scheme |

## Download

👉 [Download Latest Release](https://github.com/VenInDays/chrome-vm-android/releases/latest)

## Installation

1. Download the APK from [Releases](https://github.com/VenInDays/chrome-vm-android/releases)
2. Enable **Install from Unknown Sources** in Android Settings
3. Install the APK
4. Open **Chr-VM** browser
5. Go to `chrome://flags` and search for extension-related flags

## Technical Details

### Native Patch
- `extensions.disabled` → `extensionx.disabled` in `libmonochrome.so`
- This removes the feature flag that disables extensions on Android

### Manifest Patch
- Package name: `com.android.chrome.vm`
- All content providers, permissions, and authorities updated
- No conflict with original Chrome installation

### Extension Pre-install
- Violentmonkey v2.36.0 (CRX3) extracted and placed in `assets/extensions/violentmonkey/`

### Signing
- Keystore: RSA 2048-bit
- V2 + V3 APK Signature Scheme verified

## Based On
- Chrome v138.0.7204.179
- Target: Android 8+ (API 26+)
- Architecture: armeabi-v7a

## ⚠️ Disclaimer
This project is for **educational and research purposes only**. 
Chrome is a trademark of Google LLC. This mod is not affiliated with or endorsed by Google.
