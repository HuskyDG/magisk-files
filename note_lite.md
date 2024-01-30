## R65B92427-kitsune-lite (26404)

> Lite version is inspired from MagiskLite, has no Zygisk supported

- In Magisk in whitelist mode, all applications are hidden by default. Only applications checked in the su list can obtain super user permissions.
- For most applications, only the main process will request su. Do not select all processes, as this will affect performance.
- Use the log system to monitor process startup, and installation of devices with abnormal log systems is prohibited.
-  Always enforce SuList mode. Removed Zygisk functionality. Module functionality is not supported and most modules are expected to break the system.
- Other changes synchronized with R65B8FE82-kitsune (26404)