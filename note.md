## R657C2E65-kitsune (26403)

**💣 CAUTION! You are using a version of Magisk that is not approved by the official Magisk developer. This version may have risky changes that could damage your device or expose your data. Do not ask for any support or report any problems to the official Magisk channels. If you are using this version without knowing it is unofficial, please switch to the official Magisk at [github.com/topjohnwu/Magisk](https://github.com/topjohnwu/Magisk). USE THIS AT YOUR OWN RISK!**

- Update to ca25935 (26403)

### Diffs to official Magisk

- [App] Added a new feature to install Magisk into `/system` partition for emulators that do not have a boot image.
- [Zygisk] Changed the method of injecting zygote process from native bridge to ptrace implementation: attach init to monitor for the zygote process and then inject into zygote after attaching. The implementation comes from [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext). This method is realiable and more compatible with some emulators that ignore `ro.dalvik.vm.native.bridge` property. However, it required Android 8+
- [General] Enhanced the support for mounting in pre-init for modules. This enables modules to modify the system before the init process starts, which can be useful for some advanced use cases.
- [General] Implemented a new feature to support deleting file by using indicated whiteout character device, similar to `overlayfs`. This allows modules to delete files from the original system without actually modifying it.
- [Zygisk] Added support for GrepheneOS Android 14, a privacy and security focused mobile OS with Android app compatibility. This is because the official Magisk does not support it.
- [General] Restored support for devices with no selinux support, which was removed by the official Magisk. This allows users to use Magisk on devices that do not have selinux enabled in kernel.

### Magisk upstream level

- HEAD commit: ca25935