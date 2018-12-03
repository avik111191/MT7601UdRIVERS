MT7601UdRIVERS

osboxes@osboxes:~/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS$ make
make -C tools
make[1]: Entering directory '/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/tools'
gcc -g bin2h.c -o bin2h
make[1]: Leaving directory '/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/tools'
/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/tools/bin2h
cp -f os/linux/Makefile.6 /home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux/Makefile
make -C /lib/modules/4.15.0-39-generic/build SUBDIRS=/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux modules
make[1]: Entering directory '/usr/src/linux-headers-4.15.0-39-generic'
Makefile:975: "Cannot use CONFIG_STACK_VALIDATION=y, please install libelf-dev, libelf-devel or elfutils-libelf-devel"
  CC [M]  /home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux/../../sta/sync.o
/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux/../../sta/sync.c: In function ‘PeerBeacon’:
/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux/../../sta/sync.c:2180:12: error: passing argument 8of ‘StaAddMacTableEntry’ from incompatible pointer type [-Werror=incompatible-pointer-types]
            ie_list,
            ^~~~~~~
In file included from /home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/include/rt_config.h:59:0,
                 from /home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux/../../sta/sync.c:28:
/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/include/rtmp.h:7892:9: note: expected ‘IE_LISTS * {aka struct _IE_lists *}’ but argument is of type ‘BCN_IE_LIST * {aka struct _bcn_ie_list *}’
 BOOLEAN StaAddMacTableEntry(
         ^~~~~~~~~~~~~~~~~~~
cc1: some warnings being treated as errors
scripts/Makefile.build:332: recipe for target '/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux/../../sta/sync.o' failed
make[2]: *** [/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux/../../sta/sync.o] Error 1
Makefile:1551: recipe for target '_module_/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux' failed
make[1]: *** [_module_/home/osboxes/vscodeProjects/mt7601uDrivers/MT7601u/MT7601UdRIVERS/os/linux] Error 2
make[1]: Leaving directory '/usr/src/linux-headers-4.15.0-39-generic'
Makefile:394: recipe for target 'LINUX' failed
make: *** [LINUX] Error 2
