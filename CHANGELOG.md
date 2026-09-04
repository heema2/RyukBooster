# Changelog

All notable updates to **Ryuk Booster** — app releases and catalog refreshes.

Users can also download installers from [heema2/RyukBooster](https://github.com/heema2/RyukBooster/releases) and follow the live update channel at [heema2/RyukBooster-Updates](https://github.com/heema2/RyukBooster-Updates/releases).

### Catalog v9 — 2026-09-04

- [Changed] Azan Desktop (azan_desktop): downloadUrl: "https://github.com/heema2/Azan-Desktop/releases/download/..." → "https://github.com/heema2/Azan-Desktop/releases/download/..."

### Catalog v8 — 2026-09-03

- [Changed] Azan Desktop (azan_desktop): name: "Azan Desktop v2" → "Azan Desktop"; downloadUrl: "https://github.com/heema2/Azan-Desktop/releases/download/..." → "https://github.com/heema2/Azan-Desktop/releases/download/..."

### Catalog v7 — 2026-09-03

- [Changed] Azan Desktop v2 (azan_desktop): downloadUrl: "https://drive.google.com/file/d/1JIfs7YOgJAby93cRy2jNOpS-..." → "https://github.com/heema2/Azan-Desktop/releases/download/..."

## [1.5.5] — 2026-09-03

- **PC Optimizer** (renamed from Cleaner): hero PC Health ring, Scan Now → Optimize Now flow, module checkboxes, live activity log, result cards
- **Duplicate Finder**: centered scan ring, progress animation, reclaimable stats, detailed clean summary
- **Startup Manager**: app icons, Task Manager-style impact, confirmation before remove, Removed list with Restore
- Sidebar regrouped: System / Apps / General; selected-page highlight
- **Windows Apps** + **Uninstaller** (spelling fixed); app card labels wrap fully (no more clipped chips)
- Logs: search by date/time/message, newest first; clearer application vs catalog update wording
- Update checks: every **1 hour** while running (plus launch / reconnect / Check now) — no more frequent manifest polling

## [1.5.4] — 2026-09-03

- Fixed missing Apps page logos (all catalog icons now ship in `Assets/Icons`)
- Icon loader also checks installed app executables and the local install Assets folder

### Catalog v6 — 2026-09-03

- **Changed:** Azan Desktop (azan_desktop): name: "Azan Desktop" → "Azan Desktop v2"

## [1.5.3] — 2026-09-03

- Immediate update progress popup with status and percent
- Live release-feed checks (avoids stale CDN `/latest/download` lag)
- Catalog-only GitHub releases marked as prerelease so they do not hide app updates
- Ships with catalog **v5**

### Catalog v5 — 2026-09-03

- Catalog refresh (including Azan link updates)

## [1.5.2] — 2026-09-03

- Fixed app / installer / uninstaller icons (R + apple logo)
- Shortcuts and Apps & Features use shipped `app.ico`
- Polished public GitHub README + Updates channel page

## [1.5.1] — 2026-09-03

- Settings page (theme, startup, tray, update checks)
- Single-EXE custom installer with embedded payload
- Auto-updater + catalog hot-updates over GitHub Releases

## [1.5.0] — 2026-09-02

- Initial public update-channel packaging for Ryuk Booster
