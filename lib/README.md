# Flutter Engine SO Library Directory

This directory contains custom-compiled Flutter Engine shared libraries that fix the fontconfig issue on ARM64 Linux systems.

## Available Versions

- `libflutter_linux_gtk.so.X.Y.Z` - Compiled with fontconfig support for Flutter X.Y.Z
  - Fixes: Root cause of CJK character rendering on ARM64
  - Auto-detected from app source code (.fvmrc)

## Usage

The `flutter-font-fix` script automatically:
1. Detects the app's Flutter version from GitHub source (.fvmrc)
2. Checks if a matching SO file exists in this directory
3. Mounts the SO file to replace the official one

No manual version mapping needed!

## Build Information

These libraries were compiled from Flutter Engine source with the following modifications:
- `flutter_use_fontconfig = true` in args.gn
- Target: linux-arm64
- Mode: debug/profile/release

For build instructions, see `../FONTCONFIG_BUG_INVESTIGATION.md`

## Example

```bash
# Place your compiled SO file here:
lib/libflutter_linux_gtk.so.3.35.3

# Run repair (auto-detects version):
sudo flutter-font-fix -a desktop-security-center

# Output:
# [INFO] Auto-detecting Flutter version...
#        Repository: https://github.com/canonical/desktop-security-center
#        Commit: d93b42d
#        Flutter version: 3.35.3
# [INFO] Found matching SO file!
#        SO file: libflutter_linux_gtk.so.3.35.3
# [OK] Root cause fixed with Flutter Engine replacement!
```
## Flutter 3.38.5
- Flutter Commit: f6ff1529fd6d8af5f706051d9251ac9231c83407
- Built on: 2025-12-26 07:54:34 UTC
- Size: 32M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.38.6
- Flutter Commit: 8b872868494e429d94fa06dca855c306438b22c0
- Built on: 2026-01-09 20:44:48 UTC
- Size: 32M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.38.7
- Flutter Commit: 3b62efc2a3da49882f43c372e0bc53daef7295a6
- Built on: 2026-01-14 20:44:44 UTC
- Size: 32M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.38.8
- Flutter Commit: bd7a4a6b5576630823ca344e3e684c53aa1a0f46
- Built on: 2026-01-27 20:56:22 UTC
- Size: 32M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.38.9
- Flutter Commit: 67323de285b00232883f53b84095eb72be97d35c
- Built on: 2026-01-29 21:03:56 UTC
- Size: 32M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.41.0
- Flutter Commit: 44a626f4f0027bc38a46dc68aed5964b05a83c18
- Built on: 2026-02-11 21:14:59 UTC
- Size: 33M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.41.1
- Flutter Commit: 582a0e7c5581dc0ca5f7bfd8662bb8db6f59d536
- Built on: 2026-02-13 21:04:55 UTC
- Size: 33M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.41.2
- Flutter Commit: 90673a4eef275d1a6692c26ac80d6d746d41a73a
- Built on: 2026-02-20 04:36:08 UTC
- Size: 33M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.41.3
- Flutter Commit: 48c32af0345e9ad5747f78ddce828c7f795f7159
- Built on: 2026-03-02 21:05:52 UTC
- Size: 33M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.41.4
- Flutter Commit: ff37bef603469fb030f2b72995ab929ccfc227f0
- Built on: 2026-03-04 20:46:32 UTC
- Size: 33M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions


## Flutter 3.41.5
- Flutter Commit: 2c9eb20739dfec95e2c74bd3dfa4601b0a8a36aa
- Built on: 2026-03-18 21:15:54 UTC
- Size: 33M
- Platform: Linux ARM64
- Build Type: Release
- Features: Fontconfig enabled
- Built by: GitHub Actions

