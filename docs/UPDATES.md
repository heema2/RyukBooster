# Ryuk Booster updates (free GitHub Releases)

## One-time setup

1. Create a **public** GitHub repo (recommended name: `RyukBooster-Updates`).
2. Create a Personal Access Token with permission to create releases / upload assets.
3. Run **Ryuk Admin** (`src/RyukAdmin`) — login with your admin password.
4. Open **Settings**, enter owner, repo, and token (stored DPAPI-protected in `%AppData%\RyukAdmin\`).
5. Clients use this manifest URL (already set for `heema2`):

```json
{
  "manifestUrl": "https://github.com/heema2/RyukBooster-Updates/releases/latest/download/manifest.json"
}
```

A hard-coded fallback to the same URL is also built into the app if `update.config.json` is missing.

## Installer downloads (versioned)

Public installer repo: **https://github.com/heema2/RyukBooster/releases**

- Each app version gets tag `vX.Y.Z` with `RyukBooster-Setup-X.Y.Z.exe` (older tags stay online).
- Latest shortcut: https://github.com/heema2/RyukBooster/releases/download/latest-installer/RyukBooster-Setup-latest.exe

Build + upload:

```bat
installer\build-release.bat
powershell -File tools\publish-installer-github.ps1
```

The custom installer is a **single EXE** (payload embedded). No payload folder required.

## Publishing catalog / app updates

### Catalog only (links / apps)
1. Edit in Ryuk Admin, then **Save local**, then **Publish catalog**
2. Users online get a catalog refresh dialog and footer `Catalog updated (vN)` (not a full app reinstall)

### Full app update
1. Bump version and run `installer\build-release.bat`
2. In Admin use **Publish app update** with `dist\RyukBooster-Update.zip`
3. Also run `tools\publish-installer-github.ps1` so the public installer page stays current

## Client behavior

| State | Behavior |
|---|---|
| Offline | Footer: Offline — updates paused |
| Online + newer app | Progress popup opens immediately, downloads, installs, restarts |
| Online + newer catalog | Progress popup opens immediately with download bar, then Finished |
| Check now (Settings) | Progress popup opens immediately while checking |
| Online + up to date | Footer: You have the latest version |
| Back online / every ~60s / Apps page | Automatic recheck (popup only when work is needed) |

### Admin publishing UX

Ryuk Admin confirms before **Remove**, **Save local**, **Reload**, **Publish catalog**, and **Publish app**, and shows a change summary (added / removed / field edits) so you can verify before shipping an update.


## Admin security

- Admin password is PBKDF2-verified (salted hash only).
- GitHub write token never ships inside Ryuk Booster.
- Do not put Ryuk Admin inside the public installer.
