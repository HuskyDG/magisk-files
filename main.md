# Kitsune Mask

![Delta](https://user-images.githubusercontent.com/84650617/222942594-63336f63-6a26-492e-a1d1-a356b5f777b3.png)

## Introduction

**This is not an officially supported [topjohnwu](https://github.com/topjohnwu) project**. 

> This is not Official Magisk, please [go to this page and download Official Magisk](https://github.com/topjohnwu/Magisk)

## Download

### Stable / Beta

- [26.4 Stable](https://github.com/HuskyDG/download/raw/main/magisk/26.4-kitsune.apk)

### Canary / Debug

#### Download

> Switch to debug build before report any issues

- [Canary (app-release.apk)](https://huskydg.github.io/magisk-files/app-release.apk)
- [Debug (app-debug.apk)](https://huskydg.github.io/magisk-files/app-debug.apk) 
- [Source code](https://github.com/HuskyDG/magisk) 
- [Changelog](https://github.com/HuskyDG/magisk-files/blob/main/note.md)

## How to install

### How do I install Kitsune Mask from scratch?

Process like installing Magisk: <https://topjohnwu.github.io/Magisk/install.html>

### How do I switch from the current Magisk to Kitsune Mask and vice versa?

Easy, just do it like when you update Magisk!

#### Direct Install (Recommended)

1. Install, open, and then grant root access to Kitsune Mask.
2. Inside **Magisk**, tap "Install" and then "Direct Install". If you don't see this, try restarting the app.

#### Or flash Kitsune Mask from the current Magisk app

1. Rename the extension `magisk.apk` to `magisk.zip`
2. Open Magisk app, click the "Modules" tab -> "Install from storage" and choose `magisk.zip`

#### Install Magisk directly to `/system` instead of patching boot image (Not recommended)

This method is only for ROMs with Permissive SELinux mode or Enforcing SELinux with permissive "u:r:su:s0" context in sepolicy rules, such as user-debug ROMs like LineageOS. Make sure you have a backup of your ROM and a working Custom Recovery. Your ROM and kernel must support read-write mounting and dynamic SeLinux rules patching. This method may cause boot failure, so use it at your own risk!

1. Restore the stock boot image if you have Magisk installed already.
2. Boot to recovery, rename `magisk.apk` to `systemmagisk.zip`, and flash it.
3. To update Magisk, use **Direct Install into system partition** instead of **Direct Install**.

### How to install Magisk into Android emulator

Patching ramdisk is not feasible for the emulator, as the ramdisk partition has insufficient space for Magisk binaries. The following emulators and Android-x86 projects have been tested: NoxPlayer, LDPlayer, MEmu, BlissOS, and PrimeOS.

#### Step-by-step to install Magisk into an emulator like NoxPlayer, LDPlayer, MemuPlayer, etc

1. Enable Root access in emulator settings.
2. Install and open Kitsune Mask.
3. Grant root access to Kitsune Mask, click "Install" under the Magisk field, and use "Direct Install into system partition" option instead of "Direct Install" option. (If you don't see this option, close and re-open Kitsune Mask app.) Don't restart now!
4. Backup built-in `su` (`/system/bin/su` and `/system/xbin/su`) and delete them (in case you want to uninstall Magisk and restore to built-in `su`), then reboot. Because emulators like LDPlayer will remove any `su` after disabling ROOT from settings, **DO NOT** disable Root access in emulator settings.
5. Enjoy Magisk!

#### Step-by-step instructions for installing Magisk on Bluestacks

1. Download Bluestacks Tweaker [here](https://bstweaker.ru).
2. Use Bluestacks Tweaker and click "Unlock" to unlock Bluestacks instance, and then launch it. Otherwise, you can't install Magisk.
3. When the instance starts up successfully, click "Patch" to open root access, install Kitsune Mask, and execute the "Direct Install into system partition" action.
4. When you are done, click "UnPatch" and then restart the instance.
5. Enjoy Magisk!

## Donate me

- Paypal: [paypal.me/huskydg](http://paypal.me/huskydg)
- Thanks for all your supports and hope you have a good day! 👍

## Other links

- [Telegram group](https://t.me/kitsun3m4gisk)

## Credits

- Magisk author: [topjohnwu](https://github.com/topjohnwu/magisk)
- Magisk contributors: [vvb2060](https://github.com/vvb2060), [yujincheng08](https://github.com/yujincheng08), [RikkaW](https://github.com/RikkaW), [canyie](https://github.com/canyie)
- Zygisk implementation by ptrace: [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext),  [Dr-TSNG](https://github.com/Dr-TSNG/ZygiskNext) and [5ec1cff](https://github.com/5ec1cff)

## License

Our license obviously is the same as [Magisk's license](https://github.com/topjohnwu/Magisk#License)

```
Magisk, including all git submodules are free software:
you can redistribute it and/or modify it under the terms of the
GNU General Public License as published by the Free Software Foundation,
either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
```