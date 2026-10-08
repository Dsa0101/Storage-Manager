# 🚀 Storage Manager — Roadmap & Development Cycle

Official roadmap for **Storage Manager**, following the standard `X.Y.Z` versioning convention.

---

## 📌 Versioning Convention (`X.Y.Z`)

- **`X` (Major):** Radical UI redesign + massive core feature overhaul (e.g., `2.0.0`).
- **`Y` (UI/Features):** User interface updates, new navigation elements, and primary feature additions.
- **`Z` (Patch/Logic):** Bug fixes, backend logic optimization, minor tweaks, and visual polish.

---

## 🗺️ Current Roadmap

### 🟢 Version 1.2.7 — Visual Refinement & Animations
- [x] **UI Polish:** Redesigned disk sunburst/donut charts, updated navigation panels, and improved Settings view.
- [ ] **Algorithm Polish:** Optimized disk scanning engine for low CPU/memory overhead on large volumes.
- [ ] **Animation System:** Fluid UI animation engine with toggleable performance modes in Preferences.

---

### 🟡 Version 1.2.8 — Advanced Modes, Plugins & Changelog
- [ ] **Public Beta Cycle:** Community testing for 1.2.8 features ahead of final release.
- [ ] **Real-Time Visual Scan:**
  * Interactive live scan mode sorted by file size.
  * Optional toggle in Settings (retains lightweight classic spinner when off).
- [ ] **Integrated CMD Console (Disabled by default):**
  * Power-user command palette.
  * Script execution for UI tweaks and system tasks.
  * Official command wiki documentation.
- [ ] **Plugin System:** Infrastructure allowing users to build and load custom modules.
- [ ] **In-App Changelog:** Native *"What's New"* panel to track update notes and version history.
- [ ] **Inter-Process Integration (IPC):** Bridge setup for companion external app integration.

---

## 🔴 Future Vision — Version 2.0.0 (Major Release)
- [ ] Final leap to 2.0.0 featuring mature UI, optimized logic, and production stability.
- [ ] Codebase review and submission for official Merge Request.
- [ ] Official release on the **Droplet Store**.

---

> **Note:** Daily development takes place in private **Nightly builds** using the `droppykit` source code. Beta and stable releases are compiled separately for public distribution.
