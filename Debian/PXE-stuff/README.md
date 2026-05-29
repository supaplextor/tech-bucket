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
```
