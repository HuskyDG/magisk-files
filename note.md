## R655F6129-kitsune

Welcome back Delta users!

### Diffs to official Magisk

- [Zygisk] New way to load Zygisk, like [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext) project
- [General] Add MagiskHide back from Magisk v23.0 with minor improvement
- [General] Add SuList, whitelist based hide
- [General] Support mounting in pre-init for modules
- [General] Support install Magisk into system partition (for emulators)
- [resetprop] Don't always deleting read-only properties before setting them

### Credits
- [Ptrace init based Zygisk](https://github.com/HuskyDG/Magisk/commits/ptrace-zygisk), we are using part of code from [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext) writing by [Dr-TSNG](https://github.com/Dr-TSNG/ZygiskNext) and [5ec1cff](https://github.com/5ec1cff). Credits was adding to code as well. 
- ZygiskNext is an open source project licensed under GPL-v3.0, which provides standalone implementation of Zygisk and Zygisk API support for KernelSU and a replacement of Magisk's built-in Zygisk.

### Magisk upstream level

- HEAD commit: ecb31ee

> This version might have bugs, please using Official Magisk instead