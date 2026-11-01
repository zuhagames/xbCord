<p align="center">
  <img src="assets/xbcord-banner.svg" width="720" alt="xbCord — Discord for Xbox 360">
</p>

<h3 align="center">Discord on Xbox 360.</h3>

<p align="center">
  Open Discord from the Xbox guide to read messages,<br>
  chat with friends and browse your servers.
</p>

<p align="center">
  <a href="https://github.com/zuhagames/xbCord/releases/tag/v0.2.1"><img src="https://img.shields.io/badge/version-0.2.1%20beta-93c83d" alt="Version 0.2.1 beta"></a>
  <img src="https://img.shields.io/badge/platform-Xbox%20360-107c10" alt="Platform: Xbox 360">
  <a href="#updating"><img src="https://img.shields.io/badge/updates-in%20app-5865f2" alt="In-app updates"></a>
  <a href="https://github.com/zuhagames/xbCord/releases"><img src="https://img.shields.io/github/downloads/zuhagames/xbCord/total?label=downloads&amp;color=93c83d" alt="Total GitHub release downloads"></a>
  <a href="https://discord.gg/eCE87fsmaV"><img src="https://img.shields.io/badge/community-Discord-5865f2?logo=discord&amp;logoColor=white" alt="Join Zuha Games - Official Server"></a>
</p>

<p align="center">
  <a href="https://github.com/zuhagames/xbCord/releases/download/v0.2.1/xbCord.beta.0.2.1.zip"><img src="https://img.shields.io/badge/Download%20ZIP-Beta%200.2.1-93c83d?style=for-the-badge&amp;logo=github&amp;logoColor=white" alt="Download xbCord Beta 0.2.1 ZIP"></a>
</p>

<p align="center">
  <a href="#installation">Installation</a> ·
  <a href="#features">Features</a> ·
  <a href="https://github.com/zuhagames/xbCord/releases/tag/v0.2.1">Release notes</a> ·
  <a href="#help">Help</a> ·
  <a href="https://discord.gg/eCE87fsmaV">Discord support</a>
</p>

## Download xbCord

**[Download Beta 0.2.1](https://github.com/zuhagames/xbCord/releases/download/v0.2.1/xbCord.beta.0.2.1.zip)** — everything you need is in the ZIP, including the installation guide.

Use this download rather than **Code → Download ZIP**. Extract it on your PC before copying the folders to your USB.

You'll need an Xbox 360 that can already load plugins, such as through DashLaunch. xbCord is currently in beta, so keep a backup of your existing setup.

## Installation

1. Copy **`Plugins`** and **`xbCord`** from the extracted folder to the root of your USB. Include everything inside `Plugins\xbCord`, including `slot-a`.
2. In DashLaunch, select `Usb:\Plugins\xbCord\xbCord.xex` in a free plugin slot and save. Don't load xbCord twice.
3. Restart with the USB connected. Open the Xbox guide, go to Games & Apps and select **xbCord**. Choose **Type the token**, or put your token in `xbCord\token.txt` and choose **Log in from USB**. Replace all the placeholder text with just your token on one line.

**Updating an existing install?** Keep your `xbCord.ini`, `token.bin` and `state.txt`. Don't replace your saved token with the placeholder. If you're copying over a version that already has the updater, back up and replace the whole `Plugins\xbCord` folder. Keep your separate `xbCord` data folder.

<details>
<summary><strong>How the folders should look</strong></summary>

```text
USB root/
├── Plugins/
│   └── xbCord/
│       ├── xbCord.xex              ← choose this in DashLaunch
│       ├── xbCord.xur
│       └── slot-a/                 ← keep all files inside
│           ├── xbCord-core.xex
│           ├── xbCord.xur
│           ├── release.manifest
│           ├── release.sig
│           └── ready.marker
└── xbCord/
    ├── xbCord.ini
    └── token.txt                   ← replace the placeholder to sign in
```

xbCord creates `token.bin`, `state.txt` and its logs when needed. Keep the USB connected while using it.

`slot-a` contains the plugin itself. The XEX outside it is the loader. Updates go into the other slot so the previous version is still there if startup fails. Don't delete the slot folder or select its core XEX in DashLaunch.

</details>

The full setup guide is **[INSTALL-XBCORD.txt](INSTALL-XBCORD.txt)**. It's also in the ZIP.

## Features

- Read and send messages in your DMs and server channels.
- Search chats, servers and channels by name, or filter for unread messages.
- Pin your favorite chats, servers and channels. Rename the shortcuts and put them in your own order.
- Send quick replies like “Hi!” or “Be right back.” You can edit the phrases in Settings.
- Edit or delete your own messages.
- Choose what notifications show: the message, just the sender, or “New Discord message.”
- Find out why a connection failed with the diagnostics screen.
- Download updates from inside xbCord.

### Controller shortcuts

| Button | What it does |
| --- | --- |
| **LS click** | Search the current list. In Pinned, rename or move a shortcut. |
| **BACK** | Toggle unread-only. Press **B** to clear filters. |
| **START** | Pin or unpin the selected chat, server or channel. |
| **X** in a chat | Choose a quick message. |
| **A** on your message | Open its options, including edit and delete. |

## Updating

Once you've installed the complete package, you can get future updates from xbCord:

1. Open **Settings → Updates → Check for updates**.
2. Choose **Download update** and wait for **“Update downloaded and verified.”**
3. Restart when you're ready, then leave xbCord running for at least **one minute**.

Your account data and settings stay in place. The previous plugin slot is kept as a fallback if the new version doesn't finish starting. xbCord won't restart the console for you.

Leave `update_channel=beta` in `xbCord/xbCord.ini` for normal beta releases.

<details>
<summary><strong>Developer updater test — 0.2.0.1</strong></summary>

[0.2.0.1 updater test](https://github.com/zuhagames/xbCord/releases/tag/v0.2.0.1-dev.1) is for trying the upgrade to 0.2.1. Install its complete package, leave `update_channel=dev` in the INI, then open **Settings → Updates**.

If you just want to use xbCord, grab 0.2.1 at the top of this page.

</details>

## Help

Need help, found a bug or have a suggestion? Join **[Zuha Games - Official Server](https://discord.gg/eCE87fsmaV)**. That's where you'll find xbCord support and updates on our other projects too.

- **Can't connect?** Open Connection diagnostics from Settings or the sign-in screen. It can tell you whether the problem is DNS, the connection, authentication or verification.
- **Discord asks for verification?** Complete it in the official Discord app, then use Retry sign-in in xbCord's Account help.
- **Need to disable xbCord?** Put an empty `xbCord_off.txt` at the USB root and restart. Remove it to enable xbCord again.

If you're sharing logs for support, don't include your token or token files. More setup and recovery help is in the [installation guide](INSTALL-XBCORD.txt).

---

<p align="center">
  <strong>Made by zuha | zec2235</strong><br>
  Published by <a href="https://github.com/zuhagames">ZuhaGames</a>
</p>
