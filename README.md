# Vibe Manifest

Manifest repository for building Vibe Android ROM based on LineageOS 23.2 (Android 16).

## Getting Started

To initialize your local repository using the Vibe manifest:

```bash
repo init -u https://github.com/Vibe-Android/android_manifest.git -b lineage-23.2
```

Then sync the sources:

```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

## Vibe Customizations

The manifest inherits all standard LineageOS 23.2 repositories while overriding the following active Vibe components:

- `vendor/vibe` -> `Vibe-Android/android_vendor_vibe`
- `packages/apps/VibeParts` -> `Vibe-Android/android_packages_apps_VibeParts`
- `packages/apps/Settings` -> `Vibe-Android/android_packages_apps_Settings`
- `frameworks/base` -> `Vibe-Android/android_frameworks_base`
