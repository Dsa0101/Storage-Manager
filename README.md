# Storage Manager

A [Droppy](https://getdroppy.app) droplet that puts three disk tools right beside your notch, on the shelf.

- **Monitor** — see used and free space for your startup disk and every mounted external volume at a glance, with animated rings and bars that turn red as a disk fills up.
- **Smart Cleanup** — scans Downloads, Desktop, user Caches and the Trash, lists the heaviest items, and lets you empty the Trash or clear caches in one tap. Destructive actions always ask for confirmation first, and nothing is deleted without it.
- **Offload** — drag files or folders onto the drop zone and Storage Manager copies them to a mounted external drive, verifies the copy byte-for-byte before touching the original, and only then frees the internal file. If the copy doesn't match, the original is left untouched.

It also includes a **Settings** tab with interface language (System / Spanish / English), a customizable accent color, sound feedback, auto-refresh, and control over how many heavy items are listed.

Made by **Dsa** · version **1.2.5**

> **Source code repository:** not published yet. The GitHub link for this droplet's code will be shared shortly — I'll add it as soon as it's up.

## Requirements

- macOS on Apple Silicon or Intel, running **Droppy 15.3.0** or newer.
- DroppyKit ABI 1, min API 1.19.0.

## Surfaces

- `shelf-widget` — the main entry point on the expanded shelf (solo and paired layouts).
- `expanded-surface` — a full takeover panel on the notch, opened from the shelf widget.

## Build

The droplet must be built with the official SDK script so it links against the resilient `DroppyKit.framework` that Droppy ships. A bare `swift build` produces a bundle the app refuses to load.

```bash
# clone the SDK next to this package (first time only)
git clone https://gitlab.com/droppyformac1/droppykit.git sdk

# build, sign and strip quarantine
./build.sh
```

The bundle lands at `.build/AppCleanerNotch.droplet`.

## Install

Local (unsigned) builds are loaded by Droppy only after you approve them in the app:

1. Open Droppy → **Settings** → **Droplet Store** → **Local droplets**.
2. Choose **Add** and select `.build/AppCleanerNotch.droplet`.
3. Accept the "untrusted build" prompt.

Droppy then registers the droplet and shows the **Storage Manager** widget on the shelf.

## Layout

```
AppCleanerNotch/
├── droplet.json            # manifest: id, version, creator, surfaces, icon
├── build.sh                # wraps sdk/Scripts/build-droplet.sh + codesign + xattr
├── StorageManager.icon/    # Icon Composer document (icon.json + Assets)
├── Assets/Creator.png      # creator avatar shown in the Store
└── Sources/AppCleanerNotch/
    └── AppCleanerNotch.swift   # droplet, store and all SwiftUI surfaces
```

## License

See repository once published (link above).
