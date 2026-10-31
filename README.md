# xbCord Beta 0.2.1

Published by **ZuhaGames**. Made by **zuha | zec2235**.

Download [0.2.1](https://github.com/zuhagames/xbCord/releases/tag/v0.2.1), or the [0.2.0.1 developer updater test](https://github.com/zuhagames/xbCord/releases/tag/v0.2.0.1-dev.1). This repository distributes plugin builds.

- Search chats, servers and channels: click **LS** to search names in the current list.
- Connection diagnostics: view DNS, TCP, TLS, authentication and verification results from Settings or the sign-in screen.
- Organize pinned shortcuts: click **LS** in Pinned to rename or move favorites up/down.
- Unread-only filter: press **BACK** in chats, servers or channels. **B** clears active filters.
- Edit/delete your own messages: select a message and press **A**. Deletion asks for confirmation.
- Notification privacy: choose preview, sender only or “New Discord message” under Settings.

Copy the complete `Plugins` and `xbCord` folders to your USB root. Keep `launch.ini` pointing to `Usb:\Plugins\xbCord\xbCord.xex`. Install the whole plugin folder including `slot-a`; the entry XEX is a loader. Preserve existing token, state and settings in the separate data folder. For a manual upgrade from another loader build, back up and replace the complete plugin folder so old slot-selection records are not carried over. Read [INSTALL-XBCORD.txt](INSTALL-XBCORD.txt).

Open **Settings > Updates** to check and download. Signed metadata and file hashes are verified before staging the inactive slot. Restart when convenient and allow at least one minute for startup confirmation. An unconfirmed startup falls back at the next boot. Updates never force a restart or replace account data.

Use `update_channel=beta` in `xbCord/xbCord.ini` for beta releases, or `dev` for developer builds. Both feeds currently offer 0.2.1, allowing the 0.2.0.1 developer test to upgrade. GitHub update requests contain no Discord account credentials. xbCord account requests go directly to Discord.

The SDK build and PC simulations passed. Physical Xbox boot, upgrade and recovery testing remains required; these releases are marked as prereleases. Keep a complete previous installation on your PC for manual recovery. Never share token files.
