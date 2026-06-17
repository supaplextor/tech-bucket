```
# mt -f /dev/sa0 status
mt: /dev/sa0: Device not configured

root@bsd-1:/usr/src # make buildkernel KERNCONF=TAPE3 && make installkernel KERNCONF=TAPE3

```
* man 4 sa

```
root@bsd-1:/boot # cat /usr/src/sys/amd64/conf/TAPE3 
include GENERIC
ident TAPE3

device sa

options ZFS
device zfs
(redundant; same as GENERIC)
root@bsd-1:~ # ls -l /dev/sa* /dev/nsa* /dev/st* /dev/nst*
ls: /dev/nst*: No such file or directory
crw-rw----  1 root operator 0x7e Jun 16 17:45 /dev/nsa0
crw-rw----  1 root operator 0x7d Jun 16 17:45 /dev/sa0
crw-rw----  1 root operator 0x7c Jun 16 17:45 /dev/sa0.ctl
lrwxr-xr-x  1 root wheel       4 Jun 16 17:45 /dev/stderr -> fd/2
lrwxr-xr-x  1 root wheel       4 Jun 16 17:45 /dev/stdin -> fd/0
lrwxr-xr-x  1 root wheel       4 Jun 16 17:45 /dev/stdout -> fd/1
root@bsd-1:~ # 

root@bsd-1:~ #     camcontrol devlist
<QUANTUM DLT-V4 0A00>              at scbus0 target 5 lun 0 (sa0,pass0)
<Patriot Burst SBFM61.3>           at scbus2 target 0 lun 0 (pass1,ada0)
<AHCI SGPIO Enclosure 2.00 0001>   at scbus3 target 0 lun 0 (ses0,pass2)
<KVM vmDisk-CD 0.01>               at scbus4 target 0 lun 0 (pass3,cd0)
<USB SanDisk 3.2Gen1 1.00>         at scbus5 target 0 lun 0 (pass4,da0)

sa0 at ahc0 bus 0 scbus0 target 5 lun 0
sa0: <QUANTUM DLT-V4 0A00> Removable Sequential Access SCSI-2 device
sa0: Serial Number MYL7M00075
sa0: 40.000MB/s transfers (20.000MHz, offset 8, 16bit)

```


