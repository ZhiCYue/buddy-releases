<div align="center">
  <img src="logo.png" width="120" alt="Buddy" />
  <h1>Buddy</h1>
  <p>An AI agent companion that lives in your menu bar —<br/>each agent is a desktop pet you click to chat with.</p>
</div>

## Download

Grab the installer for your platform from the **[latest release](../../releases/latest)**:

| Platform | File |
|----------|------|
| macOS (Apple Silicon / M-series) | `Buddy-<version>-arm64.dmg` |
| Windows | `Buddy-<version>-x64.exe` |
| Linux | `Buddy-<version>-x86_64.AppImage` |

## Install

### macOS

1. Open the `.dmg`, drag **Buddy** into **Applications**, then eject the disk image.
2. Buddy has no Dock icon — after launching, look for it in the **menu bar** at the top of the screen.

If the first launch says **"Buddy is damaged and can't be opened"**, run these two commands in **Terminal**, then open it again:

```bash
xattr -cr /Applications/Buddy.app
codesign --force --deep --sign - /Applications/Buddy.app
```

> On Intel Macs the first command is usually enough; on Apple Silicon run both.

### Windows

Double-click `Buddy-<version>-x64.exe` to install. If SmartScreen blocks it, click **More info → Run anyway**. Buddy lives in the **system tray** (bottom-right of the taskbar).

### Linux

Make the AppImage executable, then run it:

```bash
chmod +x Buddy-<version>-x86_64.AppImage
./Buddy-<version>-x86_64.AppImage
```

> Some desktop environments (e.g. GNOME) need an AppIndicator/StatusNotifier extension for the tray icon to show up.

## Usage

- Click the menu-bar / tray icon to create, edit, or show/hide your agents.
- Click a desktop pet to chat with its agent; right-click to close it.
- Add your model API key in settings to get started.

---

Found a bug? Open an [issue](../../issues).
