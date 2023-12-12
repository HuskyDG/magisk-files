## R6578316E-kitsune (26402)

**💣 CAUTION! You are using a version of Magisk that is not approved by the official Magisk developer. This version may have risky changes that could damage your device or expose your data. Do not ask for any support or report any problems to the official Magisk channels. If you are using this version without knowing it is unofficial, please switch to the official Magisk at [github.com/topjohnwu/Magisk](https://github.com/topjohnwu/Magisk). USE THIS AT YOUR OWN RISK!**

- Upsteam to f7e4716 (26402)

### Diffs to official Magisk

- [App] Added a new feature to install Magisk into `/system` partition for emulators that do not have a boot image. This allows users to root their emulators without modifying the kernel or the ramdisk.
- [Zygisk] Changed the method of injecting zygote process by using ptrace implementation from [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext), it is an open source project written by [Dr-TSNG](https://github.com/Dr-TSNG/ZygiskNext) and [5ec1cff](https://github.com/5ec1cff). This is more reliable and compatible with some emulators that ignore `ro.dalvik.vm.native.bridge` property.
- [General] Enhanced the support for mounting in pre-init for modules. This enables modules to modify the system before the init process starts, which can be useful for some advanced use cases.
- [General] Implemented a new feature to support deleting file by using indicated whiteout character device, similar to `overlayfs`. This allows modules to delete files from the original system without actually modifying it.
- [Zygisk] Added support for GrepheneOS Android 14, a privacy and security focused mobile OS with Android app compatibility. This is because the official Magisk does not support it.
- [General] Restored support for devices with no selinux support, which was removed by the official Magisk. This allows users to use Magisk on devices that do not have selinux enabled.

### Magisk upstream level

- HEAD commit: f7e4716