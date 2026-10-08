<div align="center">

# 🐶 Mopsino Account Manager

**Roblox multi-account manager, tracker and automation toolkit for Windows.**

[![Release](https://img.shields.io/github/v/release/kildreyn/mopsino-account-manager?style=flat-square&label=release&color=ef4444)](https://github.com/kildreyn/mopsino-account-manager/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/kildreyn/mopsino-account-manager/total?style=flat-square&label=downloads&color=22c55e)](https://github.com/kildreyn/mopsino-account-manager/releases)
[![Windows](https://img.shields.io/badge/OS-Windows-0078D4?style=flat-square&logo=windows11&logoColor=white)](https://github.com/kildreyn/mopsino-account-manager/releases/latest)
[![Auto Update](https://img.shields.io/badge/updates-automatic-8b5cf6?style=flat-square)](https://github.com/kildreyn/mopsino-account-manager/releases)

<p align="center">
  <a href="https://github.com/kildreyn/mopsino-account-manager/releases/download/v1.1.0/MopsinoAccountManager-Setup-1.1.0.exe">
    <img src="https://img.shields.io/badge/DOWNLOAD%20SETUP-v1.1.0-2ea44f?style=for-the-badge&logo=windows11&logoColor=white" alt="Download Mopsino Account Manager Setup">
  </a>
</p>

<p align="center"><b>Direct installer download — no scrolling through release notes.</b></p>

</div>

---

> [!IMPORTANT]
> **Official Mopsino downloads are published only in this repository.**
>
> Download the installer from **Releases**. Do not download repacked builds from random mirrors or third-party links.

## Mopsino Account Manager

Mopsino Account Manager is a Windows desktop application for managing multiple Roblox accounts from one place.

It combines account launching, multi-instance support, account status monitoring, automatic reconnect, script/webhook tracking, farm analytics, drop history, customization and in-app updates in one interface.

### Main features

- **Multi-account launcher** — launch several Roblox accounts with configurable delay.
- **Multi-instance support** — built into Mopsino; no separate MultiRoblox executable is required.
- **Account Status** — view Roblox online / in-game status without PRO.
- **Account Tracker** — PRO tracker for script webhook data, farm statistics, safety state and drops.
- **Auto-Reconnect** — automatically reconnect tracked accounts after a disconnect/crash.
- **Webhook Tracker** — local endpoint for supported scripts with optional Discord forwarding.
- **Drop tracking** — rarity priority, account attribution, highlighted rare drops and session/history views.
- **Compact Roblox window** — resize launched Roblox windows to a compact 800×600 layout.
- **Customization** — themes, custom backgrounds and interface colors.
- **Automatic updates** — Mopsino checks, downloads and installs new versions from GitHub Releases.
- **Private device/license handling** — sensitive identifiers stay outside the renderer where possible.

## Installation

1. Open the **Latest Release**.
2. Download `MopsinoAccountManager-Setup-x.x.x.exe`.
3. Run the installer.
4. Launch **Mopsino Account Manager** from the desktop or Start Menu.

### Updates

Mopsino has a built-in updater. When a newer version is available, the application can show release notes, download the update and install it after restart.

You normally do **not** need to download every new version manually.

## Tracker webhook

For scripts that support a custom webhook URL, use the local Mopsino receiver:

```text
http://localhost:3217/mopsino
```

Mopsino can parse account stats, safety/ban status, rewards and drops, then optionally forward the original webhook to Discord.

## Safety

Mopsino stores sensitive account/session data locally. Never share your Roblox session cookies, authentication tickets, license secrets or private configuration files with other people.

> [!NOTE]
> Mopsino Account Manager is an independent project and is not affiliated with Roblox Corporation.

## Links

- **Download setup:** https://github.com/kildreyn/mopsino-account-manager/releases/download/v1.1.0/MopsinoAccountManager-Setup-1.1.0.exe
- **Latest release:** https://github.com/kildreyn/mopsino-account-manager/releases/latest
- **All releases:** https://github.com/kildreyn/mopsino-account-manager/releases
- **Discord:** invite will be added after the official server setup is finished.

---

<div align="center">

**Mopsino Account Manager**

Built for a cleaner multi-account Roblox workflow.

</div>
