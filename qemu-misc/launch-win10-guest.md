```
/usr/bin/qemu-system-x86_64 \
    -monitor stdio \
    -cpu max \
    -audiodev alsa,id=snd0 \
    -device ich9-intel-hda \
    -device hda-duplex,audiodev=snd0 \
    -M pc-q35-7.1 \
    -machine accel=kvm \
    -m 8192 \
    -hda "/home/supaplex/.aqemu/Windows_10_x64_HDA.img" \
    -cdrom "/media/supaplex/ssd-windows-isos/vs_2019_enterprise.iso" \
    -boot order=c,menu=off \
    -netdev bridge,br=br0,id=net0 \
    -device e1000,netdev=net0 \
    -rtc base=localtime \
    -name "Windows 10 x64"
```
