```
root@ssr120-debian1:/server/tftp/amd64# ls /srv/tftp/amd64/debian-live/
filesystem.packages  filesystem.squashfs  initrd.img  initrd.img-6.12.57+deb13-amd64  vmlinuz  vmlinuz-6.12.57+deb13-amd64
root@ssr120-debian1:/server/tftp/amd64# grep /srv/tftp/amd64/debian-live/ /etc/exports 
/srv/tftp/amd64/debian-live/ *(ro,no_subtree_check)
root@ssr120-debian1:/server/tftp/amd64# 
```
