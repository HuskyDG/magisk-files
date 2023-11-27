## R656426A5-kitsune

**WARNING! You are using an unofficial version of Magisk that is not officially supported by the Magisk author. This version may contain unstable modifications that could harm your device or compromise your security. Do not report any issues or request any help from official Magisk channels. If you use this version but do not know this is an unofficial version, please switch to the official Magisk at github.com/topjohnwu/Magisk**

- Use unix domain socket communication
- Always inject magisk bins to `/system/bin`
- Always use `/sbin` as the magisk tmp when using the magisk installation method into `/system`

### Diffs to official Magisk

- [Zygisk] Inject zygote by ptrace init (*)
- [General] Use MagiskHide to hide when Zygisk is disabled
- [General] Support mounting in pre-init for modules
- [General] Support install Magisk into `/system` (for emulators)

### Credits

- (*) Kitsune Mask is using some code from [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext), it is an open source project written by [Dr-TSNG](https://github.com/Dr-TSNG/ZygiskNext) and [5ec1cff](https://github.com/5ec1cff) and licensed under GPL-version 3.0. [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext) offers a standalone implementation of Zygisk and Zygisk API support for KernelSU and replaces Magisk’s built-in Zygisk.

### Magisk upstream level

- HEAD commit: ecb31ee