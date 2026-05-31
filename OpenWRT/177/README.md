```root@OpenWrt:/mnt# opkg install usbutils
Installing usbutils (017-r1) to root...
Downloading https://downloads.openwrt.org/releases/24.10.5/packages/arm_cortex-a7_neon-vfpv4/packages/usbutils_017-r1_arm_cortex-a7_neon-vfpv4.ipk
Failed to send request: Operation not permitted
Collected errors:
 * opkg_download: Failed to download https://downloads.openwrt.org/releases/24.10.5/packages/arm_cortex-a7_neon-vfpv4/packages/usbutils_017-r1_arm_cortex-a7_neon-vfpv4.ipk, wget returned 4.
 * opkg_download: Check your network settings and connectivity.

 * opkg_install_pkg: Failed to download usbutils. Perhaps you need to run 'opkg update'?
 * opkg_install_cmd: Cannot install package usbutils.
```
