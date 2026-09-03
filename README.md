<p align="center">
  <img src="docs/assets/logo.png" alt="Ryuk Booster" width="128" height="128"/>
</p>

<h1 align="center">Ryuk Booster</h1>

<p align="center">
  <strong>Windows Booster for Windows 10 &amp; 11</strong><br/>
  Install essential apps silently, clean junk, manage startup, and keep your PC ready in minutes.
</p>

<p align="center">
  <a href="https://github.com/heema2/RyukBooster/releases/download/latest-installer/RyukBooster-Setup-latest.exe">
    <img src="https://img.shields.io/badge/Download-Latest%20Installer-C62A2A?style=for-the-badge&logo=windows&logoColor=white" alt="Download"/>
  </a>
  &nbsp;
  <a href="https://github.com/heema2/RyukBooster/releases">
    <img src="https://img.shields.io/badge/All%20Versions-Releases-1A1A1A?style=for-the-badge" alt="Releases"/>
  </a>
  &nbsp;
  <a href="https://github.com/heema2/RyukBooster-Updates">
    <img src="https://img.shields.io/badge/Updates%20Channel-RyukBooster--Updates-2D2D2D?style=for-the-badge&logo=github" alt="Updates"/>
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D4?logo=windows&logoColor=white" alt="Platform"/>
  <img src="https://img.shields.io/badge/Version-1.5.2-C62A2A" alt="Version"/>
  <img src="https://img.shields.io/badge/License-Proprietary-lightgrey" alt="License"/>
</p>

---

## ✨ What is Ryuk Booster?

Ryuk Booster is a dark-themed Windows utility that helps you set up and maintain a PC quickly:

| | Feature | What it does |
|---|---|---|
| <img src="docs/assets/icon-apps.svg" width="36"/> | **Apps catalog** | Browse curated apps by category, download vendor installers, install silently from local cache |
| <img src="docs/assets/icon-cleaner.svg" width="36"/> | **Cleaner** | Clear temp files, caches, and common junk to free space |
| <img src="docs/assets/icon-startup.svg" width="36"/> | **Startup manager** | Review and disable programs that slow boot |
| 🔍 | **Duplicate finder** | Find duplicate files and reclaim disk space |
| 📦 | **Unstaller** | Uninstall apps from a focused list with less clutter |
| ⚙️ | **Settings** | Theme, start with Windows, close-to-tray, update checks |
| 🔄 | **Auto updates** | Mandatory app updates + live catalog refreshes over GitHub Releases |

Close the window and the app stays in the **system tray** — use **Quit** from the tray menu when you are done.

---

## 🚀 Quick start

### 1. Download

Get the official single-file installer (always the newest build):

👉 **[RyukBooster-Setup-latest.exe](https://github.com/heema2/RyukBooster/releases/download/latest-installer/RyukBooster-Setup-latest.exe)**

Or pick a specific version from **[Releases](https://github.com/heema2/RyukBooster/releases)** (older tags stay available).

### 2. Install

1. Run the setup EXE (administrator rights are required).
2. Choose whether to create a desktop shortcut.
3. Click **Install** and wait for the progress bar to finish.
4. Launch **Ryuk Booster** from the Start Menu or desktop.

### 3. First run

1. Open **Apps** and pick what you need (browsers, runtimes, utilities, etc.).
2. Download → then install from the local cache (silent where supported).
3. Use **Cleaner** / **Startup** / **Duplicates** as needed.
4. Check the footer for update status (`You have the latest version`, catalog updates, or offline).

---

## 📖 Feature guide

### 🏠 Home
Overview of your catalog size, categories, and a quick jump into app selection.

### 🧹 Cleaner
Scan and remove temporary files and other safe junk. Review what will be cleaned before confirming.

### 🚀 Startup
List apps registered to run at logon. Disable entries you do not need to speed up boot.

### 🔍 Duplicate finder
Search folders for duplicate files, then delete the copies you do not want to keep.

### 📱 Apps & Install
- Browse by category with icons
- Download official/vendor packages into a local cache
- Queue installs and watch progress
- Desktop shortcuts are created when the vendor provides them (or when a known EXE is found)

### 🗑️ Unstaller
Focused uninstall list for removing software without hunting through Windows Settings.

### 📋 Logs
See what Ryuk Booster did (downloads, installs, cleanups) for troubleshooting.

### ⚙️ Settings
| Option | Description |
|---|---|
| Theme | Light / dark appearance |
| Start with Windows | Launch at logon |
| Close to tray | Closing the window hides to tray instead of quitting |
| Auto-check updates | Poll for app + catalog updates |
| Check now | Force an immediate update check |

### ℹ️ About
Version info and support links.

---

## 🔄 Updates

Ryuk Booster checks a public updates channel automatically.

| Channel | Repo | Purpose |
|---|---|---|
| **Installers (this repo)** | [heema2/RyukBooster](https://github.com/heema2/RyukBooster) | Versioned setup EXEs + this documentation |
| **Live updates** | [heema2/RyukBooster-Updates](https://github.com/heema2/RyukBooster-Updates) | `manifest.json`, catalog hot-updates, app update zips |

👉 Visit the updates repo anytime: **[RyukBooster-Updates](https://github.com/heema2/RyukBooster-Updates)**

### How updates behave

| State | What you see |
|---|---|
| Offline | Footer: *Offline — updates paused* (rechecks when you are back online) |
| Newer app version | Forced update dialog — install to continue |
| Newer catalog only | Info dialog + silent reload — footer shows *Catalog updated* |
| Up to date | Footer: *You have the latest version* |

Checks also run about every **60 seconds**, when you open **Apps**, and when the network comes back.

---

## 💾 System requirements

- Windows **10** or **11** (64-bit)
- Administrator privileges for install / some tools
- Internet connection for downloads and updates (offline use still works with cached installers)

---

## 🛟 Tips & troubleshooting

- **Already running?** Ryuk Booster is single-instance — launching again focuses the existing window (including from the tray).
- **Stuck / no window?** Start the app again; it will try to recover a hidden instance.
- **Uninstall:** Windows Settings → Apps → Ryuk Booster, or run the setup with uninstall from Apps & Features.
- **Installer is one EXE** — no extra payload folder required.
- For update channel details (maintainers), see [`docs/UPDATES.md`](docs/UPDATES.md).

---

## 🔗 Links

| | |
|---|---|
| ⬇️ Latest installer | https://github.com/heema2/RyukBooster/releases/download/latest-installer/RyukBooster-Setup-latest.exe |
| 🏷️ All releases | https://github.com/heema2/RyukBooster/releases |
| 📡 Updates channel | https://github.com/heema2/RyukBooster-Updates |
| 📘 Update docs | [docs/UPDATES.md](docs/UPDATES.md) |

---

<p align="center">
  <img src="docs/assets/logo.png" width="48" alt=""/>
  <br/>
  <sub>© 2026 Ryuk · Built for Windows 10 &amp; 11</sub>
</p>
