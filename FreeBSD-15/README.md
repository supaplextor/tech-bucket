<img width="1024" height="768" alt="rpviewer(1)" src="https://github.com/user-attachments/assets/f383523a-0454-454a-9e35-dae31a052e88" />

```
# mt -f /dev/sa0 status
mt: /dev/sa0: Device not configured

```

More on this later, but in the meantime I had to compile a kernel with sa module support.

```
supaplex@bsd-1:/usr/src/sys/amd64/conf $ diff -u GENERIC TAPE1 
--- GENERIC     2026-06-12 14:54:03.453358000 -0700
+++ TAPE1       2026-06-12 15:23:29.864015000 -0700
@@ -154,6 +154,7 @@
 device         isci                    # Intel C600 SAS controller
 device         ocs_fc                  # Emulex FC adapters
 device         pvscsi                  # VMware PVSCSI
+device         sa                      # sequential access tape drives
 
 # ATA/SCSI peripherals
 device         scbus                   # SCSI bus (required for ATA/SCSI)
supaplex@bsd-1:/usr/src/sys/amd64/conf $ 
```
