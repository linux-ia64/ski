```
root@dl380-g7:~/ski-test# bski -noconsole /usr/src/ski/ski-bootloader/ski-bootloader /boot/vmlinux-5.15.146-26c690eff0a5-ia64-ski-dirty root=/dev/sda simscsi=./sd simeth=enp3s0f0 init=/bin/bash PATH=/bin rw memblock=debug
loading /boot/vmlinux-5.15.146-26c690eff0a5-ia64-ski-dirty...
probing initramfs ...
initramfs not passed
starting kernel...
Linux version 5.15.146-26c690eff0a5-ia64-ski-dirty (root@dl380-g7) (ia64-linux-gcc (GCC) 14.0.0 20231224 (experimental), GNU ld (GNU Binutils) 2.41) #1 SMP PREEMPT Wed Jan 17 23:06:00 CET 2024
efi: EFI v1.00 by Hewlett-Packard
efi: SALsystab=0x10a510 
warning: unable to switch EFI into virtual mode (status=131)
No I/O port range found in EFI memory map, falling back to AR.KR0 (0xffffc000000)
printk: console [simcons0] enabled
memblock_reserve: [0x0000000000000000-0x000000000000005f] reserve_memory+0x3d0/0x400
memblock_reserve: [0x000000000010a5a0-0x000000000010a63f] reserve_memory+0x3d0/0x400
memblock_reserve: [0x000000000010a640-0x000000000010a68f] reserve_memory+0x3d0/0x400
memblock_reserve: [0x000000000010a690-0x000000000010a6e6] reserve_memory+0x3d0/0x400
memblock_reserve: [0x0000000004000000-0x0000000004f44b97] reserve_memory+0x3d0/0x400
memblock_add_node: [0x0000000000000000-0x000000017fffffff] nid=0 flags=0 find_memory+0xb0/0x1a0
memblock_alloc_try_nid: 262144 bytes align=0x40000 nid=-1 from=0x0000000100000000 max_addr=0x0000000000000000 find_memory+0x120/0x1a0
memblock_reserve: [0x000000017ffc0000-0x000000017fffffff] memblock_alloc_range_nid+0x1a0/0x2d0
SAL 0.1: Hewlett-Packard HP-simulator version 0.0
get_cache_info: ia64_pal_cache_summary() failed (status=-1)
PAL_VM_PAGE_SIZE failed with status=-1; defaulting to architected purge page-sizes.
memblock_alloc_try_nid: 131072 bytes align=0x10000 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 mca_bootmem+0x30/0x60
memblock_reserve: [0x000000017ffa0000-0x000000017ffbffff] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 262144 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 mmu_context_init+0x60/0x140
memblock_reserve: [0x000000017ff60000-0x000000017ff9ffff] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 262144 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 mmu_context_init+0xd0/0x140
memblock_reserve: [0x000000017ff20000-0x000000017ff5ffff] memblock_alloc_range_nid+0x1a0/0x2d0
MCA related initialization done
Zone ranges:
  DMA32    [mem 0x0000000000000000-0x00000000ffffffff]
  Normal   [mem 0x0000000100000000-0x000000017fffffff]
Movable zone start for each node
Early memory node ranges
  node   0: [mem 0x0000000000000000-0x000000017fffffff]
Initmem setup node 0 [mem 0x0000000000000000-0x000000017fffffff]
memblock_alloc_try_nid_raw: 7340032 bytes align=0x80 nid=0 from=0x0000000000000000 max_addr=0x0000000000000000 free_area_init_node+0x520/0xaf0
memblock_reserve: [0x000000017f820000-0x000000017ff1ffff] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=0 from=0x0000000000000000 max_addr=0x0000000000000000 setup_usemap+0xf0/0x160
memblock_reserve: [0x000000017f81ff80-0x000000017f81ff87] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=0 from=0x0000000000000000 max_addr=0x0000000000000000 setup_usemap+0xf0/0x160
memblock_reserve: [0x000000017f81ff00-0x000000017f81ff07] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 87 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 start_kernel+0x140/0xc90
memblock_reserve: [0x000000017f81fe80-0x000000017f81fed6] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 87 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 start_kernel+0x180/0xc90
memblock_reserve: [0x000000017f81fe00-0x000000017f81fe56] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 65536 bytes align=0x10000 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_alloc_info+0xe0/0x1e0
memblock_reserve: [0x000000017f800000-0x000000017f80ffff] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x830/0x1560
memblock_reserve: [0x000000017f81fd80-0x000000017f81fd87] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x880/0x1560
memblock_reserve: [0x000000017f81fd00-0x000000017f81fd07] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 4 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x8c0/0x1560
memblock_reserve: [0x000000017f81fc80-0x000000017f81fc83] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x910/0x1560
memblock_reserve: [0x000000017f81fc00-0x000000017f81fc07] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 320 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x12f0/0x1560
memblock_reserve: [0x000000017f81fa80-0x000000017f81fbbf] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 128 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0xa0/0x570
memblock_reserve: [0x000000017f81fa00-0x000000017f81fa7f] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 2048 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x160/0x570
memblock_reserve: [0x000000017f81f200-0x000000017f81f9ff] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 2056 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x1f0/0x570
memblock_reserve: [0x000000017f81e980-0x000000017f81f187] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 32 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x240/0x570
memblock_reserve: [0x000000017f81e900-0x000000017f81e91f] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 128 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0xa0/0x570
memblock_reserve: [0x000000017f81e880-0x000000017f81e8ff] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 8192 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x160/0x570
memblock_reserve: [0x000000017f81c880-0x000000017f81e87f] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 8200 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x1f0/0x570
memblock_reserve: [0x000000017f81a800-0x000000017f81c807] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_alloc_try_nid: 128 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x240/0x570
memblock_reserve: [0x000000017f81a780-0x000000017f81a7ff] memblock_alloc_range_nid+0x1a0/0x2d0
memblock_free: [0x000000017f800000-0x000000017f80ffff] pcpu_free_alloc_info+0x40/0x60
Built 1 zonelists, mobility grouping on.  Total pages: 98220
Kernel command line: root=/dev/sda simscsi=./sd simeth=enp3s0f0 init=/bin/bash PATH=/bin rw memblock=debug 
memblock_alloc_try_nid: 11 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 start_kernel+0x510/0xc90
memblock_reserve: [0x000000017f81a700-0x000000017f81a70a] memblock_alloc_range_nid+0x1a0/0x2d0
Unknown kernel command line parameters "PATH=/bin", will be passed to user space.
memblock_free: [0x000000017f81a700-0x000000017f81a70a] memblock_free_ptr+0x40/0x60
memblock_alloc_try_nid: 8388608 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 alloc_large_system_hash+0x220/0x860
memblock_reserve: [0x000000017f01a780-0x000000017f81a77f] memblock_alloc_range_nid+0x1a0/0x2d0
Dentry cache hash table entries: 1048576 (order: 7, 8388608 bytes, linear)
memblock_alloc_try_nid: 4194304 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 alloc_large_system_hash+0x220/0x860
memblock_reserve: [0x000000017ec1a780-0x000000017f01a77f] memblock_alloc_range_nid+0x1a0/0x2d0
Inode-cache hash table entries: 524288 (order: 6, 4194304 bytes, linear)
Sorting __ex_table...
mem auto-init: stack:all(zero), heap alloc:off, heap free:off
Leaving McKinley Errata 9 workaround enabled
Memory: 6255104K/6291456K available (11189K kernel code, 976K rwdata, 1104K rodata, 640K init, 322K bss, 36224K reserved, 0K cma-reserved)
SLUB: HWalign=128, Order=0-3, MinObjects=0, CPUs=1, Nodes=1
rcu: Preemptible hierarchical RCU implementation.
rcu: 	RCU event tracing is enabled.
rcu: 	RCU restricting CPUs from NR_CPUS=64 to nr_cpu_ids=1.
	Trampoline variant of Tasks RCU enabled.
rcu: RCU calculated value of scheduler-enlistment delay is 3 jiffies.
rcu: Adjusting geometry for rcu_fanout_leaf=16, nr_cpu_ids=1
NR_IRQS: 1024
+/-0ppm
clocksource: itc: mask: 0xffffffffffffffff max_cycles: 0x1d854df40, max_idle_ns: 1763180808480 ns
Console: colour dummy device 80x25
Calibrating delay loop... 1.25 BogoMIPS (lpj=19584)
pid_max: default: 32768 minimum: 301
Mount-cache hash table entries: 16384 (order: 1, 131072 bytes, linear)
Mountpoint-cache hash table entries: 16384 (order: 1, 131072 bytes, linear)
Boot processor id 0x0/0x0
rcu: Hierarchical SRCU implementation.
smp: Bringing up secondary CPUs ...
smp: Brought up 1 node, 1 CPU
Total of 1 processors activated (1.25 BogoMIPS).
DMI not present or invalid.
clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 59726888946093750 ns
futex hash table entries: 256 (order: -1, 32768 bytes, linear)
NET: Registered PF_NETLINK/PF_ROUTE protocol family
HugeTLB registered 256 MiB page size, pre-allocated 0 pages
SCSI subsystem initialized
clocksource: Switched to clocksource itc
NET: Registered PF_INET protocol family
IP idents hash table entries: 131072 (order: 4, 1048576 bytes, linear)
tcp_listen_portaddr_hash hash table entries: 4096 (order: 0, 65536 bytes, linear)
Table-perturb hash table entries: 65536 (order: 2, 262144 bytes, linear)
TCP established hash table entries: 65536 (order: 3, 524288 bytes, linear)
TCP bind hash table entries: 65536 (order: 4, 1048576 bytes, linear)
TCP: Hash tables configured (established 65536 bind 65536)
UDP hash table entries: 4096 (order: 1, 131072 bytes, linear)
UDP-Lite hash table entries: 4096 (order: 1, 131072 bytes, linear)
RPC: Registered named UNIX socket transport module.
RPC: Registered udp transport module.
RPC: Registered tcp transport module.
RPC: Registered tcp NFSv4.1 backchannel transport module.
ia64_pal_cache_summary=-1
------------[ cut here ]------------
WARNING: CPU: 0 PID: 1 at arch/ia64/kernel/topology.c:416 cache_sysfs_init+0x90/0xb0
Modules linked in:
CPU: 0 PID: 1 Comm: swapper/0 Not tainted 5.15.146-26c690eff0a5-ia64-ski-dirty #1

Call Trace:
 [<a000000100013c30>] show_stack.part.0+0x30/0x60
                                sp=e0000001001afbf0 bsp=e0000001001a11d0
 [<a000000100013eb0>] show_stack+0x90/0xc0
                                sp=e0000001001afbf0 bsp=e0000001001a11a0
 [<a000000100ad35a0>] dump_stack_lvl+0xa0/0xe0
                                sp=e0000001001afdc0 bsp=e0000001001a1138
 [<a000000100ad3610>] dump_stack+0x30/0x50
                                sp=e0000001001afdc0 bsp=e0000001001a10e0
 [<a000000100acb460>] __warn+0x140/0x1e0
                                sp=e0000001001afdc0 bsp=e0000001001a1090
 [<a000000100acb5c0>] warn_slowpath_fmt+0xc0/0xe0
                                sp=e0000001001afdc0 bsp=e0000001001a1028
 [<a000000100ce8ec0>] cache_sysfs_init+0x90/0xb0
                                sp=e0000001001afdf0 bsp=e0000001001a1010
 [<a00000010000a340>] do_one_initcall+0xe0/0x500
                                sp=e0000001001afdf0 bsp=e0000001001a0fd8
 [<a000000100ce2000>] kernel_init_freeable+0x410/0x4c0
                                sp=e0000001001afe30 bsp=e0000001001a0f78
 [<a000000100ad8890>] kernel_init+0x40/0x2b0
                                sp=e0000001001afe30 bsp=e0000001001a0f58
 [<a00000010000c2b0>] call_payload+0x50/0x80
                                sp=e0000001001afe30 bsp=e0000001001a0f40
---[ end trace 1bc392df5e1a6497 ]---
workingset: timestamp_bits=62 max_order=17 bucket_order=0
Installing knfsd (copyright (C) 1996 okir@monad.swb.de).
Block layer SCSI generic (bsg) driver version 0.4 loaded (major 254)
io scheduler mq-deadline registered
io scheduler kyber registered
brd: module loaded
loop: module loaded
NET: Registered PF_PACKET protocol family
simeth: v0.3
eth0: hosteth=enp3s0f0 simfd=3, HwAddr=xxxxxxxxxxxx, IRQ 49
SimSerial driver with no serial options enabled
ttyS0 at 0x03f8 (irq = 50) is a 16550
scsi host0: simulated SCSI host adapter
scsi 0:0:2:0: Direct-Access     HP       SIMULATED DISK   0.00 PQ: 0 ANSI: 2
sd 0:0:2:0: [sda] 16777216 512-byte logical blocks: (8.59 GB/8.00 GiB)
sd 0:0:2:0: [sda] Write Protect is off
sd 0:0:2:0: [sda] Asking for cache data failed
sd 0:0:2:0: [sda] Assuming drive cache: write through
sd 0:0:2:0: [sda] Attached SCSI disk
EXT4-fs (sda): warning: mounting unchecked fs, running e2fsck is recommended
EXT4-fs (sda): mounted filesystem without journal. Opts: (null). Quota mode: disabled.
VFS: Mounted root (ext4 filesystem) on device 8:0.
Freeing unused kernel memory: 640K
This architecture does not have kernel memory protection.
Run /bin/bash as init process
bash: cannot set terminal process group (-1): Inappropriate ioctl for device
bash: no job control in this shell
root@(none) / # random: crng init done
```
