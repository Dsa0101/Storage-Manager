# Storage Manager

A [Droppy](https://getdroppy.app) droplet that puts three disk tools right beside your notch, on the shelf.

- **Monitor** — see used and free space for your startup disk and every mounted external volume at a glance, featuring a clean UI that reflects system status.
- **Smart Cleanup** — scans Downloads, Desktop, user Caches, and deep Trash counts. Lists heavy items and lets you empty the Trash or clear caches safely in one tap. Destructive actions always ask for confirmation first.
- **Offload** — drag files or folders onto the drop zone and Storage Manager copies them to a mounted external drive, verifies the copy byte-for-byte before touching the original, and only then frees the internal file. If the copy doesn't match, the original is left untouched.

It also includes a **Settings** tab with an **In-App Changelog viewer**, multi-language selection (System / English / Spanish / Portuguese / French / German), customizable system & app-wide accent color tinting, sound feedback, auto-refresh, and control over how many heavy items are listed.

Made by **Dsa** · version **1.2.8**

> **Source code repository:** [https://github.com/Dsa0101/Storage-Manager](https://github.com/Dsa0101/Storage-Manager)

## Requirements

- macOS on Apple Silicon or Intel, running **Droppy 15.3.0** or newer.
- DroppyKit ABI 1, min API 1.19.0.

## Surfaces

- `shelf-widget` — the main entry point on the expanded shelf (solo and paired layouts).
- `expanded-surface` — a full takeover panel on the notch, opened from the shelf widget.
- `settings-pane` — droplet preference configuration inside Droppy settings.

## Build

The droplet must be built with the official SDK script so it links against the resilient `DroppyKit.framework` that Droppy ships. A bare `swift build` produces a bundle the app refuses to load.

```bash
# clone the SDK next to this package (first time only)
git clone [https://gitlab.com/droppyformac1/droppykit.git](https://gitlab.com/droppyformac1/droppykit.git) sdk

# build, sign and strip quarantine
./build.sh
