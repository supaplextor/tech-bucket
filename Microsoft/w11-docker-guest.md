http://127.0.0.1:8006/

docker run -it --rm \
  --name windows \
  -p 8006:8006 \
  --device=/dev/kvm \
  --device=/dev/net/tun \
  --cap-add NET_ADMIN \
  -v "/home/supaplex/windows11/windows:/storage" \
  --stop-timeout 120 \
  dockurr/windows
❯ Starting Windows for Docker v6.03...
❯ For support visit https://github.com/dockur/windows
❯ CPU: AMD Ryzen 7 7800X3D | RAM: 25/31 GB | DISK: 1 TB (ext4) | KERNEL: 6.12.111+deb13-amd64


❯ Host: 172.17.0.2/16 (f93d1e7a529e)  |  DNS: 192.168.1.1
❯ Guest: 172.30.0.2 (Windows)  |  Mode: NAT  |  MAC: 02:D2:FE:65:98:9C

❯ Booting Windows using QEMU v10.0.11...

BdsDxe: loading Boot0004 "Windows Boot Manager" from HD(1,GPT,33B196F3-C2C8-4A07-B31B-1DEE8B9CA307,0x800,0x40000)/\EFI\Microsoft\Boot\bootmgfw.efi
BdsDxe: starting Boot0004 "Windows Boot Manager" from HD(1,GPT,33B196F3-C2C8-4A07-B31B-1DEE8B9CA307,0x800,0x40000)/\EFI\Microsoft\Boot\bootmgfw.efi
❯ Windows started successfully, visit http://127.0.0.1:8006/ to view the screen...


