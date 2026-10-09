Hey everyone! Just a quick update on Storage Manager v1.3.2:

I haven't pushed the v1.3.2 source code to GitHub just yet, as I'm currently working through some performance optimization challenges to ensure it runs smoothly and efficiently across both Intel and Apple Silicon architectures.

Also, thanks to @Danny's feedback, I'm adding a filter so that large items in Smart Cleanup will only show up if they are over 1GB!

On top of that, I'm planning to build a companion updater app for Storage Manager so that you won't have to manage updates manually anymore—you'll be able to install new versions seamlessly with just a single click!

I'm ironing out these last details before re-submitting the post following the community guidelines. Thanks for all the support and feedback so far! 🚀

---

> **Update:** I'm doing the Smart Cleanup with animation!

> **Status:** Finished! :)
>

Hey everyone! Just a quick update on **Storage Manager v1.3.5**:

I'm currently working on a major update focused on performance optimizations, fluid UI redesigns, and new utility modules!

Here is a sneak peek at what’s currently in development for **v1.3.5**:

* **Fluid UI & Animations (CleanMyMac-style):** Implementing spring-based tab transitions, dynamic hover/active states across all views, and a revamped "Smart Clean" hero button with a circular progress animation.
* **Overhauled Disk Scanning Engine:** Rewriting file system indexing using Swift concurrency (`TaskGroup` / async-await) to resolve donut chart lag and ensure 60fps rendering without CPU spikes on Intel & Apple Silicon.
* **Auto-Eject for Mounted DMGs:** Integrated automatic detection and safe one-click unmounting for `.dmg` installer volumes via `NSWorkspace` / `DiskArbitration`.
* **System Trash Cleanup:** Adding a dedicated module to safely scan, preview, and empty `~/.Trash`.
* **1GB Large Item Filter:** Thanks to @Danny's feedback, adding a toggle in Smart Cleanup to quickly isolate heavy files over 1GB.
* **Expanded Localization:** Adding support for **Simplified Chinese (`zh-Hans`)** and **Hindi (`hi`)** alongside English, Spanish, Portuguese, French, and German.
* **Exclusion / Whitelist Manager:** A dedicated settings panel to ignore specific paths, code repositories, or file types during scans.

I'm actively coding, testing, and refining these features—making sure everything runs smoothly without removing any existing tools. Stay tuned for the release! 🚀

---

> **Update:** Currently integrating the UI animations and finalizing the new scanning algorithms.

> **Status:** Finished :)
