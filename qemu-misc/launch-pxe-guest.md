```
/usr/bin/qemu-system-x86_64 \
    -monitor stdio \
    -smp 8 \
    -audiodev alsa,id=snd0 \
    -device intel-hda \
    -device hda-duplex,audiodev=snd0 \
    -machine accel=kvm \
    -m 1024 \
    -boot order=n,menu=off \
    -netdev bridge,br=br0,id=net0 \
    -device virtio-net-pci,netdev=net0,mac=00:bc:d8:2c:23:9a \
    -rtc base=localtime \
    -name "pxebooter2"
```
