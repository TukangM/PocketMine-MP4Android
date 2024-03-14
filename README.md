# [PocketMine-MP](https://github.com/pmmp/PocketMine-MP)[4Android](https://github.com/TukangM/PocketMine-MP4Android) archived
# PocketMine-MP4Android was moved to new repositories ! https://github.com/Magisk-Modules-Alt-Repo/PocketMine-MP4Android
Run Minecraft Bedrock edition on android 
<details>
<summary>Click to expand to see screenshoots</summary>

![Screenshot_20240114-140951_Apps2SD PRO](https://github.com/TukangM/PocketMine-MP4Android/assets/91467886/2c3438f5-4cf6-4d08-9b6c-5e3c5b8caa56)
![Screenshot_20240113-234915_Termux](https://github.com/TukangM/PocketMine-MP4Android/assets/91467886/612e50c3-bc8a-4f72-bade-37ad2187bd76)
![Screenshot_20240114-093845_Termux](https://github.com/TukangM/PocketMine-MP4Android/assets/91467886/2c46ad81-bdc5-41ff-9dd6-61c688c1a71b)

</details>

## Installation

1. Download the latest release from the [Releases](https://github.com/TukangM/PocketMine-MP4Android/releases) page.
2. Flash the Magisk module using one of the following methods:
   - Magisk Manager:
     - Open Magisk Manager.
     - Tap on the "Modules" section.
     - Tap on the "+" button and select the downloaded pmmp Magisk module.
     - Reboot your device.
   - KernelSU:
     - Open Magisk Manager.
     - Tap on the "Modules" section
     - Tap on the "+ Install" button and select the downloaded pmmp Magisk module.
     - Reboot your device.
3. Alternatively, you can install the module using [Androidacy Module Manager](https://github.com/Androidacy/MagiskModuleManager) or [Magisk Module Repo Loader (MMRL)](https://github.com/DerGoogler/MMRL).

## Usage

1. Open a terminal emulator on your Android device, such as Termux or through ADB shell.
2. Execute the following commands:
   - Execute `su` (superuser):
     ```bash
     su
     start-pmmp
     ```
   - If you are using Termux:
     ```bash
     su
     start-pmmp
     ```
3. Optionally, if `start-pmmp` doesn't work, you can manually execute the start script by navigating to the `/data/local/pmmp` directory and running:
   ```bash
   cd /data/local/pmmp
   sh start.sh
   ```

## Workaround about port forward
You can using [Magisk Tailscaled](https://github.com/anasfanani/Magisk-Tailscaled), Tailscale Play Store, Playit.gg4Android (still development).
basicly playit-linux-aarch64 didn't run very well on android environment, need made changes or run on proot something run on ubuntu top on termux/android... using playit.gg as tunneling rn was impossible run on android environment. do run on termux with proot ubuntu core image

## Uninstall
If you decide to uninstall this module, note that the pmmp folder will not be removed. This is done to ensure that users of this module do not lose their world data, plugins, and server.properties.

## Updating
<details>

<summary>old Updating docs</summary>
If you want to update the PHP8 binaries and PocketMine-MP, you can simply update the module to the latest version. Future versions will include an update script (start-pmmp-update) to facilitate the update of the PocketMine-MP.phar binary only.
php8 using precompiled binary from here [TukangM/php8-aarch64-builds](https://github.com/TukangM/php8-aarch64-builds)
</details>

Now PocketMine-MP.phar can now be update with `update-pmmp` or run `/data/local/pmmp/update.sh`


## License
PocketMine-MP has [LGPL-3.0-1-ov-file](https://github.com/pmmp/PocketMine-MP?tab=LGPL-3.0-1-ov-file#readme) <br/>
PocketMine-MP4Android has [MIT License](https://github.com/TukangM/PocketMine-MP4Android/blob/main/LICENSE)
