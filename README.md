# Storage Manager

A Droppy droplet that puts three disk tools right beside your notch, on the shelf.

- **Monitor** — See used and free space for your startup disk and every mounted external volume at a glance, featuring a clean UI that reflects system status.
- **Smart Cleanup** — Scans Downloads, Desktop, and user Caches safely. Lists heavy items and lets you clear caches securely with a SHA-256 safety guard in one tap. Destructive actions always ask for confirmation first.
- **Offload** — Drag files or folders onto the drop zone and Storage Manager copies them to a mounted external drive, verifies the copy byte-for-byte before touching the original, and only then frees the internal file. If the copy doesn't match, the original is left untouched.

It also includes a Settings tab with an In-App Changelog viewer, multi-language selection (System / English / Spanish / Portuguese / French / German / Dutch / Simplified Chinese / Hindi), customizable system & app-wide accent color tinting, sound feedback, auto-refresh, and control over how many heavy items are listed.

Made by Dsa · version 1.3.5


---

## Requirements

- macOS on Apple Silicon or Intel, running Droppy 15.3.0 or newer.
- DroppyKit ABI 1, min API 1.19.0.

---

## Surfaces

- `shelf-widget` — The main entry point on the expanded shelf (solo and paired layouts).
- `expanded-surface` — A full takeover panel on the notch, opened from the shelf widget.
- `settings-pane` — Droplet preference configuration inside Droppy settings.
