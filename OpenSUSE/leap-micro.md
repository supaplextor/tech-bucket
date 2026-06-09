# qemu window
<img width="810" height="661" alt="image" src="https://github.com/user-attachments/assets/f023cadb-2ad6-438e-954f-1a92f53d93b8" />

# aqemu
<img width="895" height="1232" alt="image" src="https://github.com/user-attachments/assets/20bab1de-0528-426c-bbb9-7d8b9e84dac0" />

## dmesg

```
[    0.000000][    T0] Linux version 6.12.0-160000.5-default (geeko@buildhost) (gcc-13 (SUSE Linux) 13.4.0, GNU ld (GNU Binutils; SUSE Linux 16) 2.43.1.20241209-160000.2) #1 SMP PREEMPT_DYNAMIC Wed Sep 10 15:26:25 UTC 2025 (3545bbd)
[    0.000000][    T0] Command line: BOOT_IMAGE=/boot/vmlinuz-6.12.0-160000.5-default root=UUID=60441db9-1fb2-c014-07f9-10c8b6fda8f7 rd.timeout=60 rd.retry=45 console=ttyS0,115200 console=ttyS0 security=selinux selinux=1 systemd.show_status=1 net.ifnames=0 ignition.platform.id=qemu
[    0.000000][    T0] BIOS-provided physical RAM map:
[    0.000000][    T0] BIOS-e820: [mem 0x0000000000000000-0x000000000009fbff] usable
[    0.000000][    T0] BIOS-e820: [mem 0x000000000009fc00-0x000000000009ffff] reserved
[    0.000000][    T0] BIOS-e820: [mem 0x00000000000f0000-0x00000000000fffff] reserved
[    0.000000][    T0] BIOS-e820: [mem 0x0000000000100000-0x00000000bffdffff] usable
[    0.000000][    T0] BIOS-e820: [mem 0x00000000bffe0000-0x00000000bfffffff] reserved
[    0.000000][    T0] BIOS-e820: [mem 0x00000000feffc000-0x00000000feffffff] reserved
[    0.000000][    T0] BIOS-e820: [mem 0x00000000fffc0000-0x00000000ffffffff] reserved
[    0.000000][    T0] BIOS-e820: [mem 0x0000000100000000-0x000000013fffffff] usable
[    0.000000][    T0] BIOS-e820: [mem 0x000000fd00000000-0x000000ffffffffff] reserved
[    0.000000][    T0] NX (Execute Disable) protection: active
[    0.000000][    T0] APIC: Static calls initialized
[    0.000000][    T0] SMBIOS 2.8 present.
[    0.000000][    T0] DMI: QEMU Standard PC (i440FX + PIIX, 1996), BIOS 1.16.3-debian-1.16.3-2 04/01/2014
[    0.000000][    T0] DMI: Memory slots populated: 1/1
[    0.000000][    T0] Hypervisor detected: KVM
[    0.000000][    T0] kvm-clock: Using msrs 4b564d01 and 4b564d00
[    0.000000][    T0] kvm-clock: using sched offset of 107481609971 cycles
[    0.000001][    T0] clocksource: kvm-clock: mask: 0xffffffffffffffff max_cycles: 0x1cd42e4dffb, max_idle_ns: 881590591483 ns
[    0.000003][    T0] tsc: Detected 4199.992 MHz processor
[    0.075342][    T0] AGP: No AGP bridge found
[    0.076002][    T0] last_pfn = 0x140000 max_arch_pfn = 0x400000000
[    0.076031][    T0] MTRR map: 4 entries (3 fixed + 1 variable; max 19), built from 8 variable MTRRs
[    0.076033][    T0] x86/PAT: Configuration [0-7]: WB  WC  UC- UC  WB  WP  UC- WT  
[    0.076071][    T0] last_pfn = 0xbffe0 max_arch_pfn = 0x400000000
[    0.077455][    T0] found SMP MP-table at [mem 0x000f5480-0x000f548f]
[    0.077764][    T0] RAMDISK: [mem 0x1f11f000-0x2b886fff]
[    0.077768][    T0] ACPI: Early table checksum verification disabled
[    0.077770][    T0] ACPI: RSDP 0x00000000000F5290 000014 (v00 BOCHS )
[    0.077772][    T0] ACPI: RSDT 0x00000000BFFE2335 000034 (v01 BOCHS  BXPC     00000001 BXPC 00000001)
[    0.077775][    T0] ACPI: FACP 0x00000000BFFE21E9 000074 (v01 BOCHS  BXPC     00000001 BXPC 00000001)
[    0.077780][    T0] ACPI: DSDT 0x00000000BFFE0040 0021A9 (v01 BOCHS  BXPC     00000001 BXPC 00000001)
[    0.077781][    T0] ACPI: FACS 0x00000000BFFE0000 000040
[    0.077782][    T0] ACPI: APIC 0x00000000BFFE225D 000078 (v03 BOCHS  BXPC     00000001 BXPC 00000001)
[    0.077784][    T0] ACPI: HPET 0x00000000BFFE22D5 000038 (v01 BOCHS  BXPC     00000001 BXPC 00000001)
[    0.077785][    T0] ACPI: WAET 0x00000000BFFE230D 000028 (v01 BOCHS  BXPC     00000001 BXPC 00000001)
[    0.077786][    T0] ACPI: Reserving FACP table memory at [mem 0xbffe21e9-0xbffe225c]
[    0.077786][    T0] ACPI: Reserving DSDT table memory at [mem 0xbffe0040-0xbffe21e8]
[    0.077787][    T0] ACPI: Reserving FACS table memory at [mem 0xbffe0000-0xbffe003f]
[    0.077787][    T0] ACPI: Reserving APIC table memory at [mem 0xbffe225d-0xbffe22d4]
[    0.077787][    T0] ACPI: Reserving HPET table memory at [mem 0xbffe22d5-0xbffe230c]
[    0.077788][    T0] ACPI: Reserving WAET table memory at [mem 0xbffe230d-0xbffe2334]
[    0.078110][    T0] No NUMA configuration found
[    0.078111][    T0] Faking a node at [mem 0x0000000000000000-0x000000013fffffff]
[    0.078117][    T0] NODE_DATA(0) allocated [mem 0x13ffd2280-0x13fffcfff]
[    0.078384][    T0] Zone ranges:
[    0.078384][    T0]   DMA      [mem 0x0000000000001000-0x0000000000ffffff]
[    0.078385][    T0]   DMA32    [mem 0x0000000001000000-0x00000000ffffffff]
[    0.078386][    T0]   Normal   [mem 0x0000000100000000-0x000000013fffffff]
[    0.078386][    T0]   Device   empty
[    0.078387][    T0] Movable zone start for each node
[    0.078388][    T0] Early memory node ranges
[    0.078388][    T0]   node   0: [mem 0x0000000000001000-0x000000000009efff]
[    0.078389][    T0]   node   0: [mem 0x0000000000100000-0x00000000bffdffff]
[    0.078390][    T0]   node   0: [mem 0x0000000100000000-0x000000013fffffff]
[    0.078390][    T0] Initmem setup node 0 [mem 0x0000000000001000-0x000000013fffffff]
[    0.078551][    T0] On node 0, zone DMA: 1 pages in unavailable ranges
[    0.078709][    T0] On node 0, zone DMA: 97 pages in unavailable ranges
[    0.130375][    T0] On node 0, zone Normal: 32 pages in unavailable ranges
[    0.130832][    T0] ACPI: PM-Timer IO Port: 0x608
[    0.130845][    T0] ACPI: LAPIC_NMI (acpi_id[0xff] dfl dfl lint[0x1])
[    0.130870][    T0] IOAPIC[0]: apic_id 0, version 17, address 0xfec00000, GSI 0-23
[    0.130872][    T0] ACPI: INT_SRC_OVR (bus 0 bus_irq 0 global_irq 2 dfl dfl)
[    0.130873][    T0] ACPI: INT_SRC_OVR (bus 0 bus_irq 5 global_irq 5 high level)
[    0.130874][    T0] ACPI: INT_SRC_OVR (bus 0 bus_irq 9 global_irq 9 high level)
[    0.130875][    T0] ACPI: INT_SRC_OVR (bus 0 bus_irq 10 global_irq 10 high level)
[    0.130875][    T0] ACPI: INT_SRC_OVR (bus 0 bus_irq 11 global_irq 11 high level)
[    0.130877][    T0] ACPI: Using ACPI (MADT) for SMP configuration information
[    0.130878][    T0] ACPI: HPET id: 0x8086a201 base: 0xfed00000
[    0.130883][    T0] CPU topo: Max. logical packages:   1
[    0.130883][    T0] CPU topo: Max. logical dies:       1
[    0.130884][    T0] CPU topo: Max. dies per package:   1
[    0.130886][    T0] CPU topo: Max. threads per core:   1
[    0.130887][    T0] CPU topo: Num. cores per package:     1
[    0.130887][    T0] CPU topo: Num. threads per package:   1
[    0.130887][    T0] CPU topo: Allowing 1 present CPUs plus 0 hotplug CPUs
[    0.130915][    T0] kvm-guest: APIC: eoi() replaced with kvm_guest_apic_eoi_write()
[    0.130927][    T0] PM: hibernation: Registered nosave memory: [mem 0x00000000-0x00000fff]
[    0.130928][    T0] PM: hibernation: Registered nosave memory: [mem 0x0009f000-0x0009ffff]
[    0.130929][    T0] PM: hibernation: Registered nosave memory: [mem 0x000a0000-0x000effff]
[    0.130929][    T0] PM: hibernation: Registered nosave memory: [mem 0x000f0000-0x000fffff]
[    0.130930][    T0] PM: hibernation: Registered nosave memory: [mem 0xbffe0000-0xbfffffff]
[    0.130930][    T0] PM: hibernation: Registered nosave memory: [mem 0xc0000000-0xfeffbfff]
[    0.130930][    T0] PM: hibernation: Registered nosave memory: [mem 0xfeffc000-0xfeffffff]
[    0.130931][    T0] PM: hibernation: Registered nosave memory: [mem 0xff000000-0xfffbffff]
[    0.130931][    T0] PM: hibernation: Registered nosave memory: [mem 0xfffc0000-0xffffffff]
[    0.130932][    T0] [mem 0xc0000000-0xfeffbfff] available for PCI devices
[    0.130934][    T0] Booting paravirtualized kernel on KVM
[    0.130936][    T0] clocksource: refined-jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 1910969940391419 ns
[    0.133990][    T0] setup_percpu: NR_CPUS:8192 nr_cpumask_bits:1 nr_cpu_ids:1 nr_node_ids:1
[    0.135580][    T0] percpu: Embedded 93 pages/cpu s258048 r8192 d114688 u2097152
[    0.135607][    T0] kvm-guest: PV spinlocks disabled, no host support
[    0.135608][    T0] Kernel command line: BOOT_IMAGE=/boot/vmlinuz-6.12.0-160000.5-default root=UUID=60441db9-1fb2-c014-07f9-10c8b6fda8f7 rd.timeout=60 rd.retry=45 console=ttyS0,115200 console=ttyS0 security=selinux selinux=1 systemd.show_status=1 net.ifnames=0 ignition.platform.id=qemu
[    0.135677][    T0] Unknown kernel command line parameters "BOOT_IMAGE=/boot/vmlinuz-6.12.0-160000.5-default", will be passed to user space.
[    0.138704][    T0] Dentry cache hash table entries: 524288 (order: 10, 4194304 bytes, linear)
[    0.141969][    T0] Inode-cache hash table entries: 262144 (order: 9, 2097152 bytes, linear)
[    0.141991][    T0] Fallback order for Node 0: 0 
[    0.141993][    T0] Built 1 zonelists, mobility grouping on.  Total pages: 1048446
[    0.141994][    T0] Policy zone: Normal
[    0.141995][    T0] mem auto-init: stack:off, heap alloc:off, heap free:off
[    0.141997][    T0] AGP: Checking aperture...
[    0.217853][    T0] AGP: No AGP bridge found
[    0.218520][    T0] software IO TLB: area num 1.
[    0.258239][    T0] SLUB: HWalign=64, Order=0-3, MinObjects=0, CPUs=1, Nodes=1
[    0.258352][    T0] ftrace: allocating 48490 entries in 190 pages
[    0.264862][    T0] ftrace: allocated 190 pages with 6 groups
[    0.265516][    T0] Dynamic Preempt: voluntary
[    0.265789][    T0] rcu: Preemptible hierarchical RCU implementation.
[    0.265789][    T0] rcu: 	RCU event tracing is enabled.
[    0.265790][    T0] rcu: 	RCU restricting CPUs from NR_CPUS=8192 to nr_cpu_ids=1.
[    0.265791][    T0] 	Trampoline variant of Tasks RCU enabled.
[    0.265791][    T0] 	Rude variant of Tasks RCU enabled.
[    0.265791][    T0] 	Tracing variant of Tasks RCU enabled.
[    0.265792][    T0] rcu: RCU calculated value of scheduler-enlistment delay is 100 jiffies.
[    0.265792][    T0] rcu: Adjusting geometry for rcu_fanout_leaf=16, nr_cpu_ids=1
[    0.265800][    T0] RCU Tasks: Setting shift to 0 and lim to 1 rcu_task_cb_adjust=1 rcu_task_cpu_ids=1.
[    0.265801][    T0] RCU Tasks Rude: Setting shift to 0 and lim to 1 rcu_task_cb_adjust=1 rcu_task_cpu_ids=1.
[    0.265802][    T0] RCU Tasks Trace: Setting shift to 0 and lim to 1 rcu_task_cb_adjust=1 rcu_task_cpu_ids=1.
[    0.268953][    T0] NR_IRQS: 524544, nr_irqs: 256, preallocated irqs: 16
[    0.269173][    T0] rcu: srcu_init: Setting srcu_struct sizes based on contention.
[    0.269269][    T0] Console: colour dummy device 80x25
[    0.269343][    T0] printk: console [ttyS0] enabled
[    0.414177][    T0] ACPI: Core revision 20240827
[    0.415111][    T0] clocksource: hpet: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 19112604467 ns
[    0.416780][    T0] APIC: Switch to symmetric I/O mode setup
[    0.417803][    T0] x2apic enabled
[    0.418524][    T0] APIC: Switched APIC routing to: physical x2apic
[    0.420292][    T0] ..TIMER: vector=0x30 apic1=0 pin1=2 apic2=-1 pin2=-1
[    0.421387][    T0] clocksource: tsc-early: mask: 0xffffffffffffffff max_cycles: 0x3c8a5945912, max_idle_ns: 440795231168 ns
[    0.423147][    T0] Calibrating delay loop (skipped) preset value.. 8399.98 BogoMIPS (lpj=4199992)
[    0.424277][    T0] Last level iTLB entries: 4KB 512, 2MB 255, 4MB 127
[    0.425147][    T0] Last level dTLB entries: 4KB 512, 2MB 255, 4MB 127, 1GB 0
[    0.426153][    T0] Spectre V2 : Mitigation: Retpolines
[    0.426956][    T0] Spectre V1 : Mitigation: usercopy/swapgs barriers and __user pointer sanitization
[    0.427147][    T0] Spectre V2 : Spectre v2 / SpectreRSB: Filling RSB on context switch and VMEXIT
[    0.428149][    T0] x86/fpu: x87 FPU will use FXSAVE
[    0.441471][    T0] Freeing SMP alternatives memory: 40K
[    0.442148][    T0] pid_max: default: 32768 minimum: 301
[    0.443295][    T0] LSM: initializing lsm=lockdown,capability,landlock,yama,selinux,bpf,ima,evm
[    0.444293][    T0] landlock: Up and running.
[    0.445147][    T0] Yama: becoming mindful.
[    0.445809][    T0] SELinux:  Initializing.
[    0.447162][    T0] LSM support for eBPF active
[    0.448017][    T0] Mount-cache hash table entries: 8192 (order: 4, 65536 bytes, linear)
[    0.448223][    T0] Mountpoint-cache hash table entries: 8192 (order: 4, 65536 bytes, linear)
[    0.552315][    T1] smpboot: CPU0: AMD QEMU Virtual CPU version 2.5+ (family: 0xf, model: 0x6b, stepping: 0x1)
[    0.554221][    T1] Performance Events: AMD PMU driver.
[    0.555048][    T1] ... version:                0
[    0.555147][    T1] ... bit width:              48
[    0.556146][    T1] ... generic registers:      4
[    0.557146][    T1] ... value mask:             0000ffffffffffff
[    0.558146][    T1] ... max period:             00007fffffffffff
[    0.559076][    T1] ... fixed-purpose events:   0
[    0.559146][    T1] ... event mask:             000000000000000f
[    0.560192][    T1] signal: max sigframe size: 1440
[    0.561206][    T1] rcu: Hierarchical SRCU implementation.
[    0.561207][    T1] rcu: 	Max phase no-delay instances is 400.
[    0.563456][    T1] smp: Bringing up secondary CPUs ...
[    0.564154][    T1] smp: Brought up 1 node, 1 CPU
[    0.564158][    T1] smpboot: Total of 1 processors activated (8399.98 BogoMIPS)
[    0.576686][   T25] node 0 deferred pages initialised in 10ms
[    0.577152][    T1] Memory: 3796260K/4193784K available (16384K kernel code, 3070K rwdata, 13716K rodata, 4164K init, 6248K bss, 392620K reserved, 0K cma-reserved)
[    0.578310][    T1] devtmpfs: initialized
[    0.579191][    T1] x86/mm: Memory block size: 128MB
[    0.580569][    T1] clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 1911260446275000 ns
[    0.581149][    T1] futex hash table entries: 256 (order: 2, 16384 bytes, linear)
[    0.582237][    T1] pinctrl core: initialized pinctrl subsystem
[    0.582420][    T1] PM: RTC time: 16:13:36, date: 2026-06-09
[    0.585282][    T1] NET: Registered PF_NETLINK/PF_ROUTE protocol family
[    0.587229][    T1] DMA: preallocated 512 KiB GFP_KERNEL pool for atomic allocations
[    0.588157][    T1] DMA: preallocated 512 KiB GFP_KERNEL|GFP_DMA pool for atomic allocations
[    0.589158][    T1] DMA: preallocated 512 KiB GFP_KERNEL|GFP_DMA32 pool for atomic allocations
[    0.590156][    T1] audit: initializing netlink subsys (disabled)
[    0.591187][   T28] audit: type=2000 audit(1781046816.156:1): state=initialized audit_enabled=0 res=1
[    0.592227][    T1] thermal_sys: Registered thermal governor 'fair_share'
[    0.592232][    T1] thermal_sys: Registered thermal governor 'bang_bang'
[    0.593148][    T1] thermal_sys: Registered thermal governor 'step_wise'
[    0.594148][    T1] thermal_sys: Registered thermal governor 'user_space'
[    0.595162][    T1] cpuidle: using governor ladder
[    0.597150][    T1] cpuidle: using governor menu
[    0.598240][    T1] acpiphp: ACPI Hot Plug PCI Controller Driver version: 0.5
[    0.599331][    T1] PCI: Using configuration type 1 for base access
[    0.600196][    T1] kprobes: kprobe jump-optimization is enabled. All kprobes are optimized if possible.
[    0.619288][    T1] HugeTLB: registered 2.00 MiB page size, pre-allocated 0 pages
[    0.619292][    T1] HugeTLB: 28 KiB vmemmap can be freed for a 2.00 MiB page
[    0.623197][    T1] ACPI: Added _OSI(Module Device)
[    0.623947][    T1] ACPI: Added _OSI(Processor Device)
[    0.624148][    T1] ACPI: Added _OSI(Processor Aggregator Device)
[    0.627178][    T1] ACPI: 1 ACPI AML tables successfully acquired and loaded
[    0.628714][    T1] ACPI: Interpreter enabled
[    0.629156][    T1] ACPI: PM: (supports S0 S3 S4 S5)
[    0.630148][    T1] ACPI: Using IOAPIC for interrupt routing
[    0.631230][    T1] PCI: Using host bridge windows from ACPI; if necessary, use "pci=nocrs" and report a bug
[    0.631235][    T1] PCI: Using E820 reservations for host bridge windows
[    0.633418][    T1] ACPI: Enabled 2 GPEs in block 00 to 0F
[    0.636789][    T1] ACPI: PCI Root Bridge [PCI0] (domain 0000 [bus 00-ff])
[    0.637152][    T1] acpi PNP0A03:00: _OSC: OS supports [ASPM ClockPM Segments MSI EDR HPX-Type3]
[    0.637158][    T1] acpi PNP0A03:00: _OSC: not requesting OS control; OS requires [ExtendedConfig ASPM ClockPM MSI]
[    0.639158][    T1] acpi PNP0A03:00: fail to add MMCONFIG information, can't access extended configuration space under this bridge
[    0.640363][    T1] acpiphp: Slot [3] registered
[    0.641154][    T1] acpiphp: Slot [4] registered
[    0.642154][    T1] acpiphp: Slot [5] registered
[    0.642879][    T1] acpiphp: Slot [6] registered
[    0.643154][    T1] acpiphp: Slot [7] registered
[    0.644155][    T1] acpiphp: Slot [8] registered
[    0.645164][    T1] acpiphp: Slot [9] registered
[    0.646156][    T1] acpiphp: Slot [10] registered
[    0.646908][    T1] acpiphp: Slot [11] registered
[    0.647154][    T1] acpiphp: Slot [12] registered
[    0.648155][    T1] acpiphp: Slot [13] registered
[    0.649155][    T1] acpiphp: Slot [14] registered
[    0.649916][    T1] acpiphp: Slot [15] registered
[    0.650162][    T1] acpiphp: Slot [16] registered
[    0.651155][    T1] acpiphp: Slot [17] registered
[    0.652155][    T1] acpiphp: Slot [18] registered
[    0.653154][    T1] acpiphp: Slot [19] registered
[    0.653894][    T1] acpiphp: Slot [20] registered
[    0.654154][    T1] acpiphp: Slot [21] registered
[    0.655154][    T1] acpiphp: Slot [22] registered
[    0.656155][    T1] acpiphp: Slot [23] registered
[    0.656902][    T1] acpiphp: Slot [24] registered
[    0.657154][    T1] acpiphp: Slot [25] registered
[    0.658154][    T1] acpiphp: Slot [26] registered
[    0.659154][    T1] acpiphp: Slot [27] registered
[    0.659892][    T1] acpiphp: Slot [28] registered
[    0.660154][    T1] acpiphp: Slot [29] registered
[    0.661154][    T1] acpiphp: Slot [30] registered
[    0.662165][    T1] acpiphp: Slot [31] registered
[    0.663151][    T1] PCI host bridge to bus 0000:00
[    0.663888][    T1] pci_bus 0000:00: root bus resource [io  0x0000-0x0cf7 window]
[    0.664148][    T1] pci_bus 0000:00: root bus resource [io  0x0d00-0xffff window]
[    0.665148][    T1] pci_bus 0000:00: root bus resource [mem 0x000a0000-0x000bffff window]
[    0.666148][    T1] pci_bus 0000:00: root bus resource [mem 0xc0000000-0xfebfffff window]
[    0.667148][    T1] pci_bus 0000:00: root bus resource [mem 0xc000000000-0xc07fffffff window]
[    0.668148][    T1] pci_bus 0000:00: root bus resource [bus 00-ff]
[    0.669180][    T1] pci 0000:00:00.0: [8086:1237] type 00 class 0x060000 conventional PCI endpoint
[    0.670320][    T1] pci 0000:00:01.0: [8086:7000] type 00 class 0x060100 conventional PCI endpoint
[    0.673208][    T1] pci 0000:00:01.1: [8086:7010] type 00 class 0x010180 conventional PCI endpoint
[    0.674590][    T1] pci 0000:00:01.1: BAR 4 [io  0xc020-0xc02f]
[    0.675176][    T1] pci 0000:00:01.1: BAR 0 [io  0x01f0-0x01f7]: legacy IDE quirk
[    0.675180][    T1] pci 0000:00:01.1: BAR 1 [io  0x03f6]: legacy IDE quirk
[    0.675183][    T1] pci 0000:00:01.1: BAR 2 [io  0x0170-0x0177]: legacy IDE quirk
[    0.675185][    T1] pci 0000:00:01.1: BAR 3 [io  0x0376]: legacy IDE quirk
[    0.681334][    T1] pci 0000:00:01.3: [8086:7113] type 00 class 0x068000 conventional PCI endpoint
[    0.682162][    T1] pci 0000:00:01.3: quirk: [io  0x0600-0x063f] claimed by PIIX4 ACPI
[    0.682177][    T1] pci 0000:00:01.3: quirk: [io  0x0700-0x070f] claimed by PIIX4 SMB
[    0.685178][    T1] pci 0000:00:02.0: [1234:1111] type 00 class 0x030000 conventional PCI endpoint
[    0.686554][    T1] pci 0000:00:02.0: BAR 0 [mem 0xfd000000-0xfdffffff pref]
[    0.688677][    T1] pci 0000:00:02.0: BAR 2 [mem 0xfebd0000-0xfebd0fff]
[    0.693603][    T1] pci 0000:00:02.0: ROM [mem 0xfebc0000-0xfebcffff pref]
[    0.697270][    T1] pci 0000:00:02.0: Video device with shadowed ROM at [mem 0x000c0000-0x000dffff]
[    0.698718][    T1] pci 0000:00:03.0: [1af4:1000] type 00 class 0x020000 conventional PCI endpoint
[    0.699841][    T1] pci 0000:00:03.0: BAR 0 [io  0xc000-0xc01f]
[    0.700368][    T1] pci 0000:00:03.0: BAR 1 [mem 0xfebd1000-0xfebd1fff]
[    0.701770][    T1] pci 0000:00:03.0: BAR 4 [mem 0xc000000000-0xc000003fff 64bit pref]
[    0.702902][    T1] pci 0000:00:03.0: ROM [mem 0xfeb80000-0xfebbffff pref]
[    0.715231][    T1] ACPI: PCI: Interrupt link LNKA configured for IRQ 10
[    0.716283][    T1] ACPI: PCI: Interrupt link LNKB configured for IRQ 10
[    0.717255][    T1] ACPI: PCI: Interrupt link LNKC configured for IRQ 11
[    0.718264][    T1] ACPI: PCI: Interrupt link LNKD configured for IRQ 11
[    0.719207][    T1] ACPI: PCI: Interrupt link LNKS configured for IRQ 9
[    0.720691][    T1] iommu: Default domain type: Passthrough
[    0.721350][    T1] pps_core: LinuxPPS API ver. 1 registered
[    0.721356][    T1] pps_core: Software ver. 5.3.6 - Copyright 2005-2007 Rodolfo Giometti <giometti@linux.it>
[    0.723151][    T1] PTP clock support registered
[    0.723885][    T1] EDAC MC: Ver: 3.0.0
[    0.725401][    T1] NetLabel: Initializing
[    0.725406][    T1] NetLabel:  domain hash size = 128
[    0.725410][    T1] NetLabel:  protocols = UNLABELED CIPSOv4 CALIPSO
[    0.728167][    T1] NetLabel:  unlabeled traffic allowed by default
[    0.729150][    T1] mctp: management component transport protocol core
[    0.729158][    T1] NET: Registered PF_MCTP protocol family
[    0.731167][    T1] PCI: Using ACPI for IRQ routing
[    0.732260][    T1] pci 0000:00:02.0: vgaarb: setting as boot VGA device
[    0.732267][    T1] pci 0000:00:02.0: vgaarb: bridge control possible
[    0.732268][    T1] pci 0000:00:02.0: vgaarb: VGA device added: decodes=io+mem,owns=io+mem,locks=none
[    0.732273][    T1] vgaarb: loaded
[    0.735925][    T1] hpet: 3 channels of 0 reserved for per-cpu timers
[    0.736155][    T1] hpet0: at MMIO 0xfed00000, IRQs 2, 8, 0
[    0.736172][    T1] hpet0: 3 comparators, 64-bit 100.000000 MHz counter
[    0.741202][    T1] clocksource: Switched to clocksource kvm-clock
[    0.743740][    T1] VFS: Disk quotas dquot_6.6.0
[    0.744779][    T1] VFS: Dquot-cache hash table entries: 512 (order 0, 4096 bytes)
[    0.746097][    T1] pnp: PnP ACPI init
[    0.746968][    T1] pnp: PnP ACPI: found 6 devices
[    0.753351][    T1] clocksource: acpi_pm: mask: 0xffffff max_cycles: 0xffffff, max_idle_ns: 2085701024 ns
[    0.754958][    T1] NET: Registered PF_INET protocol family
[    0.756229][    T1] IP idents hash table entries: 65536 (order: 7, 524288 bytes, linear)
[    0.768610][    T1] tcp_listen_portaddr_hash hash table entries: 2048 (order: 3, 32768 bytes, linear)
[    0.768616][    T1] Table-perturb hash table entries: 65536 (order: 6, 262144 bytes, linear)
[    0.771432][    T1] TCP established hash table entries: 32768 (order: 6, 262144 bytes, linear)
[    0.772840][    T1] TCP bind hash table entries: 32768 (order: 8, 1048576 bytes, linear)
[    0.772877][    T1] TCP: Hash tables configured (established 32768 bind 32768)
[    0.775690][    T1] MPTCP token hash table entries: 4096 (order: 4, 98304 bytes, linear)
[    0.777274][    T1] UDP hash table entries: 2048 (order: 4, 65536 bytes, linear)
[    0.778737][    T1] UDP-Lite hash table entries: 2048 (order: 4, 65536 bytes, linear)
[    0.780062][    T1] NET: Registered PF_UNIX/PF_LOCAL protocol family
[    0.781084][    T1] NET: Registered PF_XDP protocol family
[    0.781941][    T1] pci_bus 0000:00: resource 4 [io  0x0000-0x0cf7 window]
[    0.781946][    T1] pci_bus 0000:00: resource 5 [io  0x0d00-0xffff window]
[    0.781948][    T1] pci_bus 0000:00: resource 6 [mem 0x000a0000-0x000bffff window]
[    0.781951][    T1] pci_bus 0000:00: resource 7 [mem 0xc0000000-0xfebfffff window]
[    0.781953][    T1] pci_bus 0000:00: resource 8 [mem 0xc000000000-0xc07fffffff window]
[    0.787643][    T1] pci 0000:00:01.0: PIIX3: Enabling Passive Release
[    0.787665][    T1] pci 0000:00:00.0: Limiting direct PCI/PCI transfers
[    0.787733][    T1] PCI: CLS 0 bytes, default 64
[    0.790590][   T12] Trying to unpack rootfs image as initramfs...
[    0.791553][    T1] PCI-DMA: Using software bounce buffering for IO (SWIOTLB)
[    0.791559][    T1] software IO TLB: mapped [mem 0x00000000bbfe0000-0x00000000bffe0000] (64MB)
[    0.794430][    T1] clocksource: tsc: mask: 0xffffffffffffffff max_cycles: 0x3c8a5945912, max_idle_ns: 440795231168 ns
[    0.797394][    T1] Initialise system trusted keyrings
[    0.798267][    T1] Key type blacklist registered
[    0.799091][    T1] workingset: timestamp_bits=36 max_order=20 bucket_order=0
[    0.800241][    T1] zbud: loaded
[    0.801180][    T1] integrity: Platform Keyring initialized
[    0.802074][    T1] integrity: Machine keyring initialized
[    0.802080][    T1] Allocating IMA blacklist keyring.
[    1.360005][   T12] Freeing initrd memory: 204192K
[    1.368894][    T1] Key type asymmetric registered
[    1.369676][    T1] Asymmetric key parser 'x509' registered
[    1.370586][    T1] Block layer SCSI generic (bsg) driver version 0.4 loaded (major 246)
[    1.371862][    T1] io scheduler mq-deadline registered
[    1.371865][    T1] io scheduler kyber registered
[    1.373437][    T1] io scheduler bfq registered
[    1.375020][    T1] ledtrig-cpu: registered to indicate activity on CPUs
[    1.376084][    T1] shpchp: Standard Hot Plug PCI Controller Driver version: 0.4
[    1.378071][    T1] ACPI: \_SB_.LNKC: Enabled at IRQ 11
[    1.380349][    T1] Serial: 8250/16550 driver, 32 ports, IRQ sharing enabled
[    1.382088][    T1] 00:04: ttyS0 at I/O 0x3f8 (irq = 4, base_baud = 115200) is a 16550A
[    1.384313][    T1] Non-volatile memory driver v1.3
[    1.384317][    T1] Linux agpgart interface v0.103
[    1.385898][    T1] ACPI: bus type drm_connector registered
[    1.387287][    T1] i8042: PNP: PS/2 Controller [PNP0303:KBD,PNP0f13:MOU] at 0x60,0x64 irq 1,12
[    1.389754][    T1] serio: i8042 KBD port at 0x60,0x64 irq 1
[    1.390868][    T1] serio: i8042 AUX port at 0x60,0x64 irq 12
[    1.392090][    T1] mousedev: PS/2 mouse device common for all mice
[    1.393624][    T9] input: AT Translated Set 2 keyboard as /devices/platform/i8042/serio0/input/input0
[    1.395947][    T9] input: VirtualPS/2 VMware VMMouse as /devices/platform/i8042/serio1/input/input3
[    1.397602][    T9] input: VirtualPS/2 VMware VMMouse as /devices/platform/i8042/serio1/input/input2
[    1.399106][    T1] rtc_cmos 00:05: RTC can wake from S4
[    1.400416][    T1] rtc_cmos 00:05: registered as rtc0
[    1.401293][    T1] rtc_cmos 00:05: setting system clock to 2026-06-09T16:13:36 UTC (1781021616)
[    1.402749][    T1] rtc_cmos 00:05: alarms up to one day, y3k, 242 bytes nvram, hpet irqs
[    1.404028][    T1] amd_pstate: the _CPC object is not present in SBIOS or ACPI disabled
[    1.405460][    T1] simple-framebuffer simple-framebuffer.0: [drm] Registered 1 planes with drm panic
[    1.405466][    T1] [drm] Initialized simpledrm 1.0.0 for simple-framebuffer.0 on minor 0
[    1.408389][    T1] fbcon: Deferring console take-over
[    1.408395][    T1] simple-framebuffer simple-framebuffer.0: [drm] fb0: simpledrmdrmfb frame buffer device
[    1.410715][    T1] hid: raw HID events driver (C) Jiri Kosina
[    1.412066][    T1] drop_monitor: Initializing network drop monitor service
[    1.413521][    T1] NET: Registered PF_INET6 protocol family
[    1.415224][    T1] Segment Routing with IPv6
[    1.415228][    T1] RPL Segment Routing with IPv6
[    1.416731][    T1] In-situ OAM (IOAM) with IPv6
[    1.417628][    T1] IPI shorthand broadcast: enabled
[    1.419105][    T1] sched_clock: Marking stable (1269054568, 149968586)->(1447829322, -28806168)
[    1.420529][    T1] registered taskstats version 1
[    1.421429][    T1] Loading compiled-in X.509 certificates
[    1.422330][    T1] Loaded X.509 cert 'SUSE Linux Products GmbH: ALP Secure Boot Signkey: 939dd72e1ee1ba7b2e5c14b8180da819d7822c79'
[    1.426631][    T1] Demotion targets for Node 0: null
[    1.427429][    T1] page_owner is disabled
[    1.428380][    T1] Key type .fscrypt registered
[    1.429108][    T1] Key type fscrypt-provisioning registered
[    1.431282][    T1] Key type encrypted registered
[    1.432056][    T1] ima: No TPM chip found, activating TPM-bypass!
[    1.433052][    T1] Loading compiled-in module X.509 certificates
[    1.434024][    T1] Loaded X.509 cert 'SUSE Linux Products GmbH: ALP Secure Boot Signkey: 939dd72e1ee1ba7b2e5c14b8180da819d7822c79'
[    1.435834][    T1] ima: Allocated hash algorithm: sha256
[    1.436695][    T1] ima: No architecture policies found
[    1.437538][    T1] evm: Initialising EVM extended attributes:
[    1.437541][    T1] evm: security.selinux
[    1.437543][    T1] evm: security.SMACK64 (disabled)
[    1.437545][    T1] evm: security.SMACK64EXEC (disabled)
[    1.437547][    T1] evm: security.SMACK64TRANSMUTE (disabled)
[    1.437549][    T1] evm: security.SMACK64MMAP (disabled)
[    1.437550][    T1] evm: security.apparmor
[    1.437552][    T1] evm: security.ima
[    1.437553][    T1] evm: security.capability
[    1.437555][    T1] evm: HMAC attrs: 0x1
[    1.466334][    T1] Running certificate verification RSA selftest
[    1.495631][    T1] Loaded X.509 cert 'Certificate verification self-testing key: f58703bb33ce1b73ee02eccdee5b8817518fe3db'
[    1.497636][    T1] Running certificate verification ECDSA selftest
[    1.499358][    T1] Loaded X.509 cert 'Certificate verification ECDSA self-testing key: 2900bcea1deb7bc8479a84a23d758efdfdd2b2d3'
[    1.504979][    T1] PM:   Magic number: 14:540:236
[    1.508985][    T1] RAS: Correctable Errors collector initialized.
[    1.520998][    T1] clk: Disabling unused clocks
[    1.521722][    T1] PM: genpd: Disabling unused power domains
[    1.525228][    T1] Freeing unused decrypted memory: 2028K
[    1.528498][    T1] Freeing unused kernel image (initmem) memory: 4164K
[    1.530039][    T1] Write protecting the kernel read-only data: 30720k
[    1.531057][    T1] Freeing unused kernel image (rodata/data gap) memory: 620K
[    1.558034][    T1] x86/mm: Checked W+X mappings: passed, no W+X pages found.
[    1.583981][    T1] Run /init as init process
Fatal glibc error: CPU does not support x86-64-v2
[    1.585233][    T1] Kernel panic - not syncing: Attempted to kill init! exitcode=0x00007f00
[    1.586107][    T1] CPU: 0 UID: 0 PID: 1 Comm: init Not tainted 6.12.0-160000.5-default #1 PREEMPT(voluntary) SLFO-1.2 c2fdc1668d70ca8945ee3ffae074edb3f4c70a6a
[    1.587557][    T1] Hardware name: QEMU Standard PC (i440FX + PIIX, 1996), BIOS 1.16.3-debian-1.16.3-2 04/01/2014
[    1.588613][    T1] Call Trace:
[    1.588967][    T1]  <TASK>
[    1.589279][    T1]  dump_stack_lvl+0x4b/0x70
[    1.589761][    T1]  panic+0x106/0x2d3
[    1.590187][    T1]  do_exit.cold+0x3e/0x58
[    1.590628][    T1]  ? set_pte_range+0x154/0x2c0
[    1.591135][    T1]  do_group_exit+0x30/0x80
[    1.591598][    T1]  __x64_sys_exit_group+0x18/0x20
[    1.592142][    T1]  x64_sys_call+0x17f3/0x1800
[    1.592629][    T1]  do_syscall_64+0x7d/0x160
[    1.593104][    T1]  ? do_fault+0x29f/0x5a0
[    1.593545][    T1]  ? __handle_mm_fault+0x5f9/0xee0
[    1.594065][    T1]  ? __count_memcg_events+0x53/0xf0
[    1.594635][    T1]  ? handle_mm_fault+0xb9/0x2e0
[    1.595416][    T1]  ? do_user_addr_fault+0x176/0x670
[    1.595948][    T1]  ? exc_page_fault+0x73/0x160
[    1.596464][    T1]  entry_SYSCALL_64_after_hwframe+0x76/0x7e
[    1.597100][    T1] RIP: 0033:0x7fdc1ac922a5
[    1.597555][    T1] Code: 00 00 00 00 00 90 90 90 90 90 90 90 90 90 90 90 90 90 90 f3 0f 1e fa 90 90 ba e7 00 00 00 eb 06 0f 1f 44 00 00 f4 89 d0 0f 05 <48> 3d 00 f0 ff ff 76 f3 f7 d8 89 05 8b 28 01 00 eb e9 66 0f 1f 84
[    1.599548][    T1] RSP: 002b:00007fffed7ebf18 EFLAGS: 00000206 ORIG_RAX: 00000000000000e7
[    1.600418][    T1] RAX: ffffffffffffffda RBX: 00007fdc1ac8c12e RCX: 00007fdc1ac922a5
[    1.601241][    T1] RDX: 00000000000000e7 RSI: 00007fffed7eb5e0 RDI: 000000000000007f
[    1.602064][    T1] RBP: 00007fffed7ec0f0 R08: 0000000000000001 R09: ffffffffffffffff
[    1.602872][    T1] R10: 0000000000000001 R11: 0000000000000206 R12: 00007fffed7ec0c0
[    1.603687][    T1] R13: 0000000000000000 R14: 00007fdc1ac6e000 R15: 00007fdc1ac6e548
[    1.604502][    T1]  </TASK>
[    1.604880][    T1] Kernel Offset: 0x11200000 from 0xffffffff81000000 (relocation range: 0xffffffff80000000-0xffffffffbfffffff)
[    1.612407][    T1] Rebooting in 90 seconds..


```

# fixed

Resolved by using -cpu max (kvm/qemu).
