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

The plugin is a single **`xbCord.xex`** again. The 0.2.1 name stays the same, and the 0.2.0.1 test updater can install this version.

Use this download rather than **Code → Download ZIP**. Extract it on your PC before copying the folders to your USB.

You'll need an Xbox 360 that can already load plugins, such as through DashLaunch. xbCord is currently in beta, so keep a backup of your existing setup.

## Installation

1. Copy **`Plugins`** and **`xbCord`** from the extracted folder to the root of your USB. The plugin goes at `Plugins\xbCord\xbCord.xex`.
2. In DashLaunch, select `Usb:\Plugins\xbCord\xbCord.xex` in a free plugin slot and save. Don't load xbCord twice.
3. Restart with the USB connected. Open the Xbox guide, go to Games & Apps and select **xbCord**. Choose **Type the token**, or put your token in `xbCord\token.txt` and choose **Log in from USB**. Replace all the placeholder text with just your token on one line.

**Updating an existing install?** Back up your old XEX, then replace it with the new `xbCord.xex`. Keep your `xbCord.ini`, `token.bin` and `state.txt`. Don't replace your saved token with the placeholder.

<details>
<summary><strong>How the folders should look</strong></summary>

```text
USB root/
├── Plugins/
│   └── xbCord/
│       └── xbCord.xex              ← the plugin; choose this in DashLaunch
└── xbCord/
    ├── xbCord.ini
    └── token.txt                   ← replace the placeholder to sign in
```

xbCord creates `token.bin`, `state.txt` and its logs when needed. Keep the USB connected while using it.

There's no separate loader or skin to install with this 0.2.1 package.

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
3. Once xbCord says the file has been updated, restart when you're ready.

Your account data and settings stay in place. The updater verifies the download, then replaces `xbCord.xex`. A recovery copy is kept as `xbCord.previous.bin` in your data folder. If you need it, copy that file back as `Plugins\xbCord\xbCord.xex` while the console is off. Recovery is manual in this single-file layout. xbCord won't restart the console for you.

Leave `update_channel=beta` in `xbCord/xbCord.ini` for normal beta releases.

<details>
<summary><strong>Already using the 0.2.0.1 updater test?</strong></summary>

The test download has been retired. If you already installed it, leave `update_channel=dev` in the INI and open **Settings → Updates** to get 0.2.1. Its update feed still works.

After downloading 0.2.1, restart and let it run for one minute. It will prepare the single-file plugin and ask for one more restart. Once it starts from the standalone XEX, it removes the old managed slot folders.

Keep the test build's `slot-a` until the upgrade is finished. If you already deleted it and xbCord won't start, install the new 0.2.1 XEX manually instead.

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
