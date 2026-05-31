```root@OpenWrt:/mnt# opkg install usbutils
Installing usbutils (017-r1) to root...
Downloading https://downloads.openwrt.org/releases/24.10.5/packages/arm_cortex-a7_neon-vfpv4/packages/usbutils_017-r1_arm_cortex-a7_neon-vfpv4.ipk
Failed to send request: Operation not permitted
Collected errors:
 * opkg_download: Failed to download https://downloads.openwrt.org/releases/24.10.5/packages/arm_cortex-a7_neon-vfpv4/packages/usbutils_017-r1_arm_cortex-a7_neon-vfpv4.ipk, wget returned 4.
 * opkg_download: Check your network settings and connectivity.

 * opkg_install_pkg: Failed to download usbutils. Perhaps you need to run 'opkg update'?
 * opkg_install_cmd: Cannot install package usbutils.
root@OpenWrt:/mnt# ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host 
       valid_lft forever preferred_lft forever
2: eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq state UP qlen 1000
    link/ether 26:f5:a2:0d:9d:34 brd ff:ff:ff:ff:ff:ff
    inet6 fe80::24f5:a2ff:fe0d:9d34/64 scope link 
       valid_lft forever preferred_lft forever
3: lan1@eth0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue master br-lan state LOWERLAYERDOWN qlen 1000
    link/ether 24:f5:a2:0d:9d:35 brd ff:ff:ff:ff:ff:ff
4: lan2@eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue master br-lan state UP qlen 1000
    link/ether 24:f5:a2:0d:9d:35 brd ff:ff:ff:ff:ff:ff
5: lan3@eth0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue master br-lan state LOWERLAYERDOWN qlen 1000
    link/ether 24:f5:a2:0d:9d:35 brd ff:ff:ff:ff:ff:ff
6: lan4@eth0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue master br-lan state UP qlen 1000
    link/ether 24:f5:a2:0d:9d:35 brd ff:ff:ff:ff:ff:ff
7: wan@eth0: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN qlen 1000
    link/ether 00:03:7f:ba:db:ad brd ff:ff:ff:ff:ff:ff
8: br-lan: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue state UP qlen 1000
    link/ether 24:f5:a2:0d:9d:35 brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.177/24 brd 192.168.1.255 scope global br-lan
       valid_lft forever preferred_lft forever
    inet6 fdda:f8e9:3392::1/60 scope global noprefixroute 
       valid_lft forever preferred_lft forever
    inet6 fe80::26f5:a2ff:fe0d:9d35/64 scope link 
       valid_lft forever preferred_lft forever
10: phy1-ap0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue master br-lan state UP qlen 1000
    link/ether 26:f5:a2:0d:9d:36 brd ff:ff:ff:ff:ff:ff
11: phy0-ap0: <NO-CARRIER,BROADCAST,MULTICAST,UP> mtu 1500 qdisc noqueue master br-lan state DOWN qlen 1000
    link/ether 26:f5:a2:0d:9d:38 brd ff:ff:ff:ff:ff:ff
13: phy2-ap0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue master br-lan state UP qlen 1000
    link/ether 26:f5:a2:0d:9d:37 brd ff:ff:ff:ff:ff:ff
14: phy1-ap1: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue master br-lan state UP qlen 1000
    link/ether 22:f5:a2:0d:9d:36 brd ff:ff:ff:ff:ff:ff
root@OpenWrt:/mnt# ip r
default via 192.168.1.1 dev br-lan 
192.168.1.0/24 dev br-lan scope link  src 192.168.1.177 

```
