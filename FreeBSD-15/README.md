```
root@bsd-1:~ # mt -f /dev/sa0 status
mt: /dev/sa0: Device not configured
root@bsd-1:~ # mt -f /dev/sa0 load
mt: /dev/sa0: Device not configured
```
<blockquote>You can use the /dev/rsa0.ctl device to get status when there is no tape in the drive.</blockquote>

```
root@bsd-1:~ # mt -f /dev/sa0.ctl  status
Drive: sa0: <QUANTUM DLT-V4 0A00> Serial Number: MYL7M00075
---------------------------------
Mode      Density              Blocksize      bpi      Compression
Current:  0x00:default         variable       0        enabled (IDRC)
---------------------------------
Current Driver State: at rest.
---------------------------------
Partition:  -1      Calc File Number:  -1     Calc Record Number: -1
Residual:    0  Reported File Number:  -1 Reported Record Number: -1
Flags: None
root@bsd-1:~ # mt -f /dev/sa0.ctl  load
mt: /dev/sa0.ctl: load: Device not configured

```

* man 4 sa
```
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
root@bsd-1:~ # mt -f /dev/sa0.ctl status
Drive: sa0: <QUANTUM DLT-V4 0A00> Serial Number: MYL7M00075
---------------------------------
Mode      Density              Blocksize      bpi      Compression
Current:  0x00:default         variable       0        enabled (IDRC)
---------------------------------
Current Driver State: at rest.
---------------------------------
Partition:  -1      Calc File Number:  -1     Calc Record Number: -1
Residual:    0  Reported File Number:  -1 Reported Record Number: -1
Flags: None
root@bsd-1:~ # 

<img width="1024" height="768" alt="rpviewer(4)" src="https://github.com/user-attachments/assets/a9f015f2-b983-4524-8e6b-d3139c9e4dad" />




```




