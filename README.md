# Kitsune Magisk

**This is not an officially supported [topjohnwu](https://github.com/topjohnwu) project**. 

> This is not Official Magisk, please [go to this page and download Official Magisk](https://github.com/topjohnwu/Magisk)

## Download

### Stable / Beta

- [Kitsune Mask v26.4 Stable](https://github.com/HuskyDG/download/raw/main/magisk/26.4-kitsune.apk)

### Canary / Debug

> We only accept bugreports from **LASTEST DEBUG** build. Invalid bugreports will be closed instantly.

#### Kitsune Mask

> Kitsune Mask has MagiskHide, SuList and new Zygisk loading mechanism

- [Canary (app-release.apk)](https://huskydg.github.io/magisk-files/app-release.apk)
- [Debug (app-debug.apk)](https://huskydg.github.io/magisk-files/app-debug.apk) 
- [Changelog](https://github.com/HuskyDG/magisk-files/blob/main/note.md) 

#### Kitsune Lite

> Kitsune Lite only has SuList feature and no Zygisk built-in or supported. SuList feature depends on logcat to work!

- [Canary (app-release-lite.apk)](https://huskydg.github.io/magisk-files/app-release-lite.apk)
- [Debug (app-debug-lite.apk)](https://huskydg.github.io/magisk-files/app-debug-lite.apk) 
- [Changelog](https://github.com/HuskyDG/magisk-files/blob/main/note_lite.md) 


### Other version

- [Releases page](https://github.com/HuskyDG/magisk-files/releases)

### Source code

- [https://github.com/KitsuneMagisk/magisk](https://github.com/KitsuneMagisk/magisk)  

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

Patching ramdisk is not feasible for the emulator, as the ramdisk partition has insufficient space for Magisk binaries.
The following emulators and Android-x86 projects have been tested: NoxPlayer, LDPlayer, MEmu, BlissOS, and PrimeOS.

#### Step-by-step to install Magisk into an emulator like NoxPlayer, LDPlayer, MemuPlayer, etc

1. Enable Root access in emulator settings and writable system image disk (if available)
2. Install and open Kitsune Magisk app.
3. Grant root access to Kitsune Mask, click "Install" under the Magisk field, and use "Direct Install into system partition" option instead of "Direct Install" option. (If you don't see this option, close and re-open Kitsune Mask app.)
4. Enjoy Magisk feature with Kitsune Magisk!

> For some reasons, closing Root access in emulator settings will intentionally removing Magisk `su`, so do not switch off Root access.

## Donate me

- Paypal: [paypal.me/huskydg](http://paypal.me/huskydg)
- Thanks for all your supports and hope you have a good day! 👍

## Credits

- Magisk author: [topjohnwu](https://github.com/topjohnwu/magisk)
- Magisk contributors: [vvb2060](https://github.com/vvb2060), [yujincheng08](https://github.com/yujincheng08), [RikkaW](https://github.com/RikkaW), [canyie](https://github.com/canyie)
- Magisk Hide in whitelist mode: [MagiskLite](https://t.me/magisklite)
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
