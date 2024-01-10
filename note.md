## R659E930C-kitsune (26404)

- Update resetprop to avoid increasing serial counter
- Mounting module files to system no longer need mirrors
- Add biometric authentication back
- Check full path of `init.rc`
- Grant root to shell by default (for debug build)

If you want to read changelog of previous builds, please visit [Release page](https://github.com/HuskyDG/magisk-files/releases)

### Diffs to official Magisk

Kitsune 26404+ has changed the mounting `su` location from `/system/bin` to `/apex/com.android.runtime/bin`. This is to reduce bind mount. For most apps (that don't change/hardcode `PATH` variable), this change should not break anything. An known app is Termux which hardcode `PATH` might fail to locate `su`, you can call `/debug_ramdisk/su`.

- [App] Added a new feature to install Magisk into `/system` partition for emulators that do not have a boot image.
- [Zygisk] Changed the method of loading Zygisk to ptrace init implementation (required Android 8+). The implementation comes from [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext). This method does not need to change any property and is more compatible with some emulators that ignore `ro.dalvik.vm.native.bridge` property.
- [General] Support for mounting in pre-init for modules.
- [General] Support deleting file by using indicated whiteout character device, similar to `overlayfs`
- [Zygisk] Added support for GrepheneOS Android 14, a privacy and security focused mobile OS with Android app compatibility. This is because the official Magisk does not support it.
- [General] Restored support for devices with no selinux support, which was removed by the official Magisk. This allows users to use Magisk on devices that do not have selinux enabled in kernel.
- [Module] Cancel the writable exception for `/system/etc/hosts`
- [General] Update resetprop to avoid increasing serial counter
- [Module] Mounting module files to system no longer need mirrors
- [App] Add biometric authentication back
- [General] Check full path of `init.rc`
- [General] Grant root to shell by default (for debug build)

### Magisk upstream level

- HEAD commit: 65207f96

## Magisk (65207f96) (26404)

- [SEPolicy] Update libsepol to properly set some policy config bits
- [MagiskBoot] Support compressing `init` so Magisk is installable on devices with small boot partitions
- [ResetProp] Add new wait for property feature `resetprop -w`

## Diffs to v26.4

- [Zygisk] Introduce new code injection mechanism
- [Zygisk] Support new signature introduced in U QPR2
- [SEPolicy] Update libsepol to properly set some policy config bits
- [MagiskBoot] Support compressing `init` so Magisk is installable on devices with small boot partitions