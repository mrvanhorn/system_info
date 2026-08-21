# system_info
A simple script to quickly show useful hardware information on a system
running Linux

It's output has make and model, serial number, cpu, memory, and attached
storage device information.

It does NOT show any information about any GPUs in the system.

This is a tad specific to my uses, but I thought others might find the
script useful as either an example or at least of how to get further
information about your hardware without having to be in the same room
and opening the lid.

The output looks like:

<pre>
[user@server ~]$ sudo /usr/local/bin/system_info

Hewlett-Packard HP Z220 CMT Workstation
Serial Number: 2UA3282N1N

1 x 4-core Intel(R) Xeon(R) CPU E3-1270 V2 @ 3.50GHz
with a total of 8 threads

32GB of DDR3 RAM
using 4 DIMMs with 0 empty DIMM slots

NAME               MAJ:MIN RM   SIZE RO TYPE MOUNTPOINTS
sda                  8:0    0 931.5G  0 disk 
├─sda1               8:1    0  1000M  0 part /boot/efi
├─sda2               8:2    0     2G  0 part /boot
├─sda3               8:3    0   716G  0 part 
│ ├─almalinux-root 253:0    0   200G  0 lvm  /
│ ├─almalinux-swap 253:1    0    16G  0 lvm  [SWAP]
│ └─almalinux-home 253:2    0   500G  0 lvm  /home
└─sda4               8:4    0 212.5G  0 part /vmfiles
sdb                  8:16   0 931.5G  0 disk 
├─sdb1               8:17   0 931.5G  0 part 
└─sdb9               8:25   0     8M  0 part 
sdc                  8:32   0 931.5G  0 disk 
├─sdc1               8:33   0 931.5G  0 part 
└─sdc9               8:41   0     8M  0 part 
sdd                  8:48   0   3.6T  0 disk 
├─sdd1               8:49   0    16M  0 part 
└─sdd2               8:50   0   3.6T  0 part /4tbusb
sr0                 11:0    1  1024M  0 rom  

running "AlmaLinux 9.7 (Moss Jungle Cat)"
</pre>
