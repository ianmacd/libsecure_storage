# **libsecure_storage custom kernel companion**

## Description

This Magisk module contains modified `libsecure_storage.so` libraries that allow Samsung Galaxy S9/S9+ (G960F/G965F), Tab S4 (T830/T835), and probably other rooted devices to function without losing Bluetooth pairings after reboot.

After installing this module, manually edit `/system/etc/init/secure_storage_daemon.rc` and change the line with **start secure_storage** to **stop secure_storage**. This step is not required, but will stop the secure storage daemon from running unnecessarily. This change cannot be applied systemlessly, because the file is read by the system before Magisk starts.

## Changelog

2018-09-06: v1.1

- Changed docs to include Tab S4 (T830/T835) and no longer be S9-specific.

2018-06-24: v1.0

- Initial release.
