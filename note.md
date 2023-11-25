## R6561D823-kitsune

- Revert `resetprop` changes
- Use `magiskd` to mount for SuList instead of relying on switching zygote's context `u:r:zygote:s0` to `u:r:magisk:s0`

### Diffs to official Magisk

- [Zygisk] Inject zygote by ptrace init, like [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext) project
- [General] Use MagiskHide to hide when Zygisk is off
- [General] Support mounting in pre-init for modules
- [General] Support install Magisk into system partition (for emulators)

### Credits
- [Ptrace init based Zygisk](https://github.com/HuskyDG/Magisk/commits/ptrace-zygisk): Kitsune Mask is using part of code from [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext) writing by [Dr-TSNG](https://github.com/Dr-TSNG/ZygiskNext) and [5ec1cff](https://github.com/5ec1cff). Credits to author was adding to code as well. 
- ZygiskNext is an open source project licensed under GPL-v3.0, which provides standalone implementation of Zygisk and Zygisk API support for KernelSU and a replacement of Magisk's built-in Zygisk.

### Magisk upstream level

- HEAD commit: ecb31ee

> This version might have bugs, please using Official Magisk instead