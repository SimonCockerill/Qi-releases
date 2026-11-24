# Qi releases

Installers and the update feed for **Qi**, a desktop app that runs your coding agents from one place.

This repository holds **only builds**, no source code. Qi checks it for updates and installs them itself.

## Install

- **Windows (x64):** download `Qi-Setup-<version>.exe` from [Releases](../../releases) and run it. It installs for your user only, with no admin prompt.
- **macOS (Apple Silicon):** download `Qi-<version>-macos-arm64.dmg`, drag Qi to Applications, then open it the first time with **right-click > Open**. The app isn't signed with an Apple Developer ID yet, so macOS asks once.
- **Linux:** not published here yet.

## Updates

Once Qi is installed it checks this repository in the background, downloads new versions while you work, and offers **Restart to update**. Downloads are checked against a SHA-256 in `latest.json` before anything is installed.

Releases are marked **pre-release** while they are release candidates. Qi follows release candidates by default; set `QI_UPDATE_CHANNEL=stable` to follow only promoted releases, or `QI_UPDATE_CHECK=0` to turn checking off.
