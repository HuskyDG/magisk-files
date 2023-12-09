## R6573543B-kitsune

**💣 CAUTION! You are using a version of Magisk that is not approved by the official Magisk developer. This version may have risky changes that could damage your device or expose your data. Do not ask for any support or report any problems to the official Magisk channels. If you are using this version without knowing it is unofficial, please switch to the official Magisk at [github.com/topjohnwu/Magisk](https://github.com/topjohnwu/Magisk). USE THIS AT YOUR OWN RISK!**

### Diffs to official Magisk

- [Zygisk] Inject zygote by ptrace implementation (*)
- [General] Use MagiskHide to hide when Zygisk is disabled
- [General] Support mounting in pre-init for modules
- [General] Support deleting file by using indicated whiteout character device like KSU `overlayfs`
- [App] Support install Magisk into `/system` (for emulators)
- [Daemon] Use unix socket communication
- [Zygisk] Support GrepheneOS Android 14
- [General] Support devices with no selinux support

### Credits

- (*) Kitsune Mask is using Zygisk implementation from [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext), it is an open source project written by [Dr-TSNG](https://github.com/Dr-TSNG/ZygiskNext) and [5ec1cff](https://github.com/5ec1cff) and licensed under GPL-version 3.0. [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext) offers a standalone implementation of Zygisk and Zygisk API support for KernelSU and replaces Magisk’s built-in Zygisk.

### Magisk upstream level

- HEAD commit: ecb31ee