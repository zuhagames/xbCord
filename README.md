# xbCord Beta 0.2.0.1 — developer updater test

Published by ZuhaGames. Made by zuha | zec2235.

This repository distributes xbCord plugin builds. The current build is for developers testing the GitHub updater on Xbox 360.

Copy `Plugins` and `xbCord` to your USB root. Keep `launch.ini` pointing to `Usb:\Plugins\xbCord\xbCord.xex`. Install the complete plugin folder, including `slot-a`; the entry XEX is now a small loader. Preserve your existing token, state and settings. Read [INSTALL-XBCORD.txt](INSTALL-XBCORD.txt) before installing.

Open **Settings > Updates** to check and download. A verified download is staged in the inactive slot. Restart when convenient; allow one minute for startup confirmation. The previous slot is preserved for recovery after a failed trial.

The updater uses signed metadata and file hashes. Developer checks cover interrupted downloads and failed-startup recovery, but this build still requires physical-console testing. Keep a copy of your previous installation for manual recovery.

Use `update_channel=dev` in `xbCord/xbCord.ini` for developer builds. Updates never force a restart. Never share your Discord token files.