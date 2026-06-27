```
/usr/bin/qemu-system-x86_64 \
    -monitor stdio \
    -machine accel=kvm \
    -m 512 \
    -cdrom "/home/user/public_html/AC97 WDM Driver for Windows 98.iso" \
    -hda "/home/user/.aqemu/foo.img" \
    -boot order=dc,menu=off \
    -netdev bridge,br=br0,id=net0 \
    -device rtl8139,netdev=net0 \
    -netdev bridge,br=br0,id=net1 \
    -device ne2k_isa,netdev=net1 \
    -rtc base=localtime \
    -name "winxp" \
    -device ac97,audiodev=snd0 \
    -audiodev alsa,id=snd0
```
