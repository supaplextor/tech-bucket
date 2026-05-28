```
root@ssr120-debian1:/server/tftp/amd64# ls /srv/tftp/amd64/debian-live/
filesystem.packages  filesystem.squashfs  initrd.img  initrd.img-6.12.57+deb13-amd64  vmlinuz  vmlinuz-6.12.57+deb13-amd64
root@ssr120-debian1:/server/tftp/amd64# grep /srv/tftp/amd64/debian-live/ /etc/exports 
/srv/tftp/amd64/debian-live/ *(ro,no_subtree_check)
root@ssr120-debian1:/server/tftp/amd64#

root@sky:/media/root/ssr120-debian1# mount -t nfs 192.168.1.126:/srv/tftp/amd64/debian-live/ rootfs/
root@sky:/media/root/ssr120-debian1# cd rootfs/                                                                                                                                                                                      
root@sky:/media/root/ssr120-debian1/rootfs# ls -l
total 3447400
-r--r--r-- 1 root root      69009 Nov 15  2025 filesystem.packages
-r--r--r-- 1 root root 3219841024 Nov 15  2025 filesystem.squashfs
-r--r--r-- 2 root root  143006652 Nov 15  2025 initrd.img
-r--r--r-- 2 root root  143006652 Nov 15  2025 initrd.img-6.12.57+deb13-amd64
-r--r--r-- 2 root root   12101568 Nov  5  2025 vmlinuz
-r--r--r-- 2 root root   12101568 Nov  5  2025 vmlinuz-6.12.57+deb13-amd64

root@ssr120-debian1:/srv/tftp/amd64/pxelinux.cfg# cat 01-00-ee-19-7f-62-6c 
# D-I config version 2.0
# search path for the c32 support libraries (libcom32, libutil etc.)
#path debian-installer/amd64/boot-screens/
#include debian-installer/amd64/boot-screens/menu.cfg
#default debian-installer/amd64/boot-screens/vesamenu.c32

prompt 0
timeout 0
DEFAULT live
LABEL live
        KERNEL debian-live/vmlinuz
        APPEND initrd=debian-live/initrd.img boot=live nfsroot=192.168.1.126:/srv/tftp/amd64/debian-live ethdevice-timeout=120 panic=10 noprompt noeject quiet systemd.log_level=notice splash live-media-path= netboot=nfs nfsroot=192.168.1.126:/srv/netboot/images/desktop-staff-latest

```
