---
{"dg-publish":true,"permalink":"/reuse/laptops/how-do-i-tips-and-tricks/tips/microsoft-surface-tips/"}
---



##### **Issue:** Surface 3 reboots into GRUB again after Windows install created bootable partition on internal drive.

Check BIOS boot order and attempt to boot from "Internal Storage" not "Windows Boot Manager" or "USB Device"
That should bypass the loop back and continue the install process.


