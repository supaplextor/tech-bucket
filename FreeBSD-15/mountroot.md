Mounting from zfs... failed with error 45

<img width="1024" height="768" alt="mountroot" src="https://github.com/user-attachments/assets/7c17261e-ee85-4a44-abbf-f18929847be4" />
<img width="800" height="600" alt="rpviewer(2)" src="https://github.com/user-attachments/assets/c1da435f-4f8d-4e78-8f33-6d57073a3c2a" />

# building
https://docs.freebsd.org/en/books/handbook/kernelconfig/#kernelconfig-building

# built
```
root@bsd-1:/usr/src # make buildkernel KERNCONF=TAPE3 && make installkernel KERNCONF=TAPE3
```
* man 4 sa

```
root@bsd-1:/usr/src # ls /boot/kernel*/sa*
/boot/kernel.GENERIC/safe.ko            /boot/kernel.old/safe.ko                /boot/kernel/safe.ko
/boot/kernel.GENERIC/safexcel.ko        /boot/kernel.old/safexcel.ko            /boot/kernel/safexcel.ko
root@bsd-1:/boot # cat /usr/src/sys/amd64/conf/TAPE3 
include GENERIC
ident TAPE3

device sa

options ZFS
device zfs

root@bsd-1:/boot # find . -name sa.ko
root@bsd-1:/boot # 

```
