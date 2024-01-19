```
root@dl380-g7:~/ski-test# bski -noconsole /usr/src/ski/ski-bootloader/ski-bootloader /boot/vmlinux-5.4.266-4410df70110f-ia64-ski-dirty root=/dev/sda simscsi=./sd simeth=enp3s0f0 init=/bin/bash PATH=/bin rw memblock=debug
loading /boot/vmlinux-5.4.266-4410df70110f-ia64-ski-dirty...
probing initramfs ...
initramfs not passed
starting kernel...
Linux version 5.4.266-4410df70110f-ia64-ski-dirty (root@dl380-g7) (gcc version 14.0.0 20231224 (experimental) (GCC)) #3 SMP PREEMPT Wed Jan 17 14:31:34 CET 2024
EFI v1.00 by Hewlett-Packard:
efi:  SALsystab=0x10a510 
warning: unable to switch EFI into virtual mode (status=131)
No I/O port range found in EFI memory map, falling back to AR.KR0 (0xffffc000000)
printk: console [simcons0] enabled
memblock_reserve: [0x0000000000000000-0x000000000000005f] reserve_memory+0x3d0/0x400
memblock_reserve: [0x000000000010a5a0-0x000000000010a63f] reserve_memory+0x3d0/0x400
memblock_reserve: [0x000000000010a640-0x000000000010a68f] reserve_memory+0x3d0/0x400
memblock_reserve: [0x000000000010a690-0x000000000010a6e6] reserve_memory+0x3d0/0x400
memblock_reserve: [0x0000000004000000-0x0000000004e05f1f] reserve_memory+0x3d0/0x400
memblock_alloc_try_nid: 262144 bytes align=0x40000 nid=-1 from=0x0000000100000000 max_addr=0x0000000000000000 find_memory+0x110/0x190
memblock_reserve: [0x000000017ffc0000-0x000000017fffffff] memblock_alloc_range_nid+0x180/0x2b0
SAL 0.1: Hewlett-Packard HP-simulator version 0.0
get_cache_info: ia64_pal_cache_summary() failed (status=-1)
PAL_VM_PAGE_SIZE failed with status=-1; defaulting to architected purge page-sizes.
memblock_alloc_try_nid: 131072 bytes align=0x10000 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 mca_bootmem+0x30/0x60
memblock_reserve: [0x000000017ffa0000-0x000000017ffbffff] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 262144 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 mmu_context_init+0x60/0x140
memblock_reserve: [0x000000017ff60000-0x000000017ff9ffff] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 262144 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 mmu_context_init+0xd0/0x140
memblock_reserve: [0x000000017ff20000-0x000000017ff5ffff] memblock_alloc_range_nid+0x180/0x2b0
MCA related initialization done
Zone ranges:
  DMA32    [mem 0x0000000000000000-0x00000000ffffffff]
  Normal   [mem 0x0000000100000000-0x000000017fffffff]
Movable zone start for each node
Early memory node ranges
  node   0: [mem 0x0000000000000000-0x000000017fffffff]
Initmem setup node 0 [mem 0x0000000000000000-0x000000017fffffff]
memblock_alloc_try_nid: 7340032 bytes align=0x80 nid=0 from=0x0000000000000000 max_addr=0x0000000000000000 alloc_node_mem_map.constprop.0+0xe0/0x1d0
memblock_reserve: [0x000000017f820000-0x000000017ff1ffff] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=0 from=0x0000000000000000 max_addr=0x0000000000000000 setup_usemap.constprop.0+0x100/0x170
memblock_reserve: [0x000000017f81ff80-0x000000017f81ff87] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=0 from=0x0000000000000000 max_addr=0x0000000000000000 setup_usemap.constprop.0+0x100/0x170
memblock_reserve: [0x000000017f81ff00-0x000000017f81ff07] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 87 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 start_kernel+0x120/0x9c0
memblock_reserve: [0x000000017f81fe80-0x000000017f81fed6] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 87 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 start_kernel+0x160/0x9c0
memblock_reserve: [0x000000017f81fe00-0x000000017f81fe56] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 87 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 start_kernel+0x1a0/0x9c0
memblock_reserve: [0x000000017f81fd80-0x000000017f81fdd6] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 65536 bytes align=0x10000 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_alloc_info+0xe0/0x1e0
memblock_reserve: [0x000000017f800000-0x000000017f80ffff] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x830/0x14e0
memblock_reserve: [0x000000017f81fd00-0x000000017f81fd07] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x880/0x14e0
memblock_reserve: [0x000000017f81fc80-0x000000017f81fc87] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 4 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x8c0/0x14e0
memblock_reserve: [0x000000017f81fc00-0x000000017f81fc03] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 8 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x910/0x14e0
memblock_reserve: [0x000000017f81fb80-0x000000017f81fb87] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 288 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_setup_first_chunk+0x1290/0x14e0
memblock_reserve: [0x000000017f81fa00-0x000000017f81fb1f] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 128 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0xa0/0x570
memblock_reserve: [0x000000017f81f980-0x000000017f81f9ff] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 2048 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x160/0x570
memblock_reserve: [0x000000017f81f180-0x000000017f81f97f] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 2056 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x1f0/0x570
memblock_reserve: [0x000000017f81e900-0x000000017f81f107] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 32 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x240/0x570
memblock_reserve: [0x000000017f81e880-0x000000017f81e89f] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 128 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0xa0/0x570
memblock_reserve: [0x000000017f81e800-0x000000017f81e87f] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 8192 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x160/0x570
memblock_reserve: [0x000000017f81c800-0x000000017f81e7ff] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 8200 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x1f0/0x570
memblock_reserve: [0x000000017f81a780-0x000000017f81c787] memblock_alloc_range_nid+0x180/0x2b0
memblock_alloc_try_nid: 128 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 pcpu_alloc_first_chunk+0x240/0x570
memblock_reserve: [0x000000017f81a700-0x000000017f81a77f] memblock_alloc_range_nid+0x180/0x2b0
   memblock_free: [0x000000017f800000-0x000000017f80ffff] pcpu_free_alloc_info+0x40/0x60
Built 1 zonelists, mobility grouping on.  Total pages: 98220
Kernel command line: root=/dev/sda simscsi=./sd simeth=enp3s0f0 init=/bin/bash PATH=/bin rw memblock=debug 
memblock_alloc_try_nid: 8388608 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 alloc_large_system_hash+0x240/0x960
memblock_reserve: [0x000000017f01a700-0x000000017f81a6ff] memblock_alloc_range_nid+0x180/0x2b0
Dentry cache hash table entries: 1048576 (order: 7, 8388608 bytes, linear)
memblock_alloc_try_nid: 4194304 bytes align=0x80 nid=-1 from=0x0000000000000000 max_addr=0x0000000000000000 alloc_large_system_hash+0x240/0x960
memblock_reserve: [0x000000017ec1a700-0x000000017f01a6ff] memblock_alloc_range_nid+0x180/0x2b0
Inode-cache hash table entries: 524288 (order: 6, 4194304 bytes, linear)
Sorting __ex_table...
mem auto-init: stack:off, heap alloc:off, heap free:off
Memory: 6256512K/6291456K available (10245K kernel code, 748K rwdata, 1008K rodata, 704K init, 299K bss, 34944K reserved, 0K cma-reserved)
Leaving McKinley Errata 9 workaround enabled
SLUB: HWalign=128, Order=0-3, MinObjects=0, CPUs=1, Nodes=1
rcu: Preemptible hierarchical RCU implementation.
rcu: 	RCU restricting CPUs from NR_CPUS=64 to nr_cpu_ids=1.
	Tasks RCU enabled.
rcu: RCU calculated value of scheduler-enlistment delay is 3 jiffies.
rcu: Adjusting geometry for rcu_fanout_leaf=16, nr_cpu_ids=1
NR_IRQS: 1024
+/-0ppm
clocksource: itc: mask: 0xffffffffffffffff max_cycles: 0x1d854df40, max_idle_ns: 1763180808480 ns
Console: colour dummy device 80x25
Calibrating delay loop... 1.24 BogoMIPS (lpj=19456)
pid_max: default: 32768 minimum: 301
Mount-cache hash table entries: 16384 (order: 1, 131072 bytes, linear)
Mountpoint-cache hash table entries: 16384 (order: 1, 131072 bytes, linear)
Boot processor id 0x0/0x0
rcu: Hierarchical SRCU implementation.
smp: Bringing up secondary CPUs ...
smp: Brought up 1 node, 1 CPU
Total of 1 processors activated (1.24 BogoMIPS).
DMI not present or invalid.
clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 59726888946093750 ns
futex hash table entries: 256 (order: -1, 32768 bytes, linear)
NET: Registered protocol family 16
HugeTLB registered 256 MiB page size, pre-allocated 0 pages
SCSI subsystem initialized
Registered efivars operations
clocksource: Switched to clocksource itc
NET: Registered protocol family 2
IP idents hash table entries: 131072 (order: 4, 1048576 bytes, linear)
tcp_listen_portaddr_hash hash table entries: 4096 (order: 0, 65536 bytes, linear)
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
WARNING: CPU: 0 PID: 1 at arch/ia64/kernel/topology.c:417 cache_sysfs_init+0x90/0xb0
Modules linked in:
CPU: 0 PID: 1 Comm: swapper/0 Not tainted 5.4.266-4410df70110f-ia64-ski-dirty #3

Call Trace:
 [<a000000100013050>] show_stack.part.0+0x30/0x60
                                sp=e0000001001afbf0 bsp=e0000001001a10e0
 [<a000000100013200>] show_stack+0x80/0xa0
                                sp=e0000001001afbf0 bsp=e0000001001a10c0
 [<a0000001009efe40>] dump_stack+0x110/0x150
                                sp=e0000001001afdc0 bsp=e0000001001a1050
 [<a0000001009e6a50>] __warn+0x150/0x200
                                sp=e0000001001afdc0 bsp=e0000001001a1008
 [<a0000001009e6bc0>] warn_slowpath_fmt+0xc0/0xe0
                                sp=e0000001001afdc0 bsp=e0000001001a0fa0
 [<a000000100bd8b20>] cache_sysfs_init+0x90/0xb0
                                sp=e0000001001afdf0 bsp=e0000001001a0f88
 [<a00000010000a2d0>] do_one_initcall+0x90/0x500
                                sp=e0000001001afdf0 bsp=e0000001001a0f58
 [<a000000100bd1b40>] kernel_init_freeable+0x3b0/0x500
                                sp=e0000001001afe30 bsp=e0000001001a0ef8
 [<a0000001009f06a0>] kernel_init+0x20/0x280
                                sp=e0000001001afe30 bsp=e0000001001a0ed8
 [<a00000010000c2b0>] call_payload+0x50/0x80
                                sp=e0000001001afe30 bsp=e0000001001a0ec0
---[ end trace 7d1c348ecd2591fc ]---
workingset: timestamp_bits=62 max_order=17 bucket_order=0
Installing knfsd (copyright (C) 1996 okir@monad.swb.de).
Block layer SCSI generic (bsg) driver version 0.4 loaded (major 254)
io scheduler mq-deadline registered
io scheduler kyber registered
EFI Time Services Driver v0.4
brd: module loaded
loop: module loaded
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
NET: Registered protocol family 17
sd 0:0:2:0: [sda] Attached SCSI disk
EXT4-fs (sda): warning: mounting unchecked fs, running e2fsck is recommended
EXT4-fs (sda): mounted filesystem without journal. Opts: (null)
VFS: Mounted root (ext4 filesystem) on device 8:0.
Freeing unused kernel memory: 704K
This architecture does not have kernel memory protection.
Run /bin/bash as init process
bash: cannot set terminal process group (-1): Inappropriate ioctl for device
bash: no job control in this shell
root@(none) / # random: crng init done
```
