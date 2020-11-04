# Ubuntu

# CPU 的一些基本信息

> lscpu

```
Architecture:        x86_64
CPU op-mode(s):      32-bit, 64-bit
Byte Order:          Little Endian
CPU(s):              4
On-line CPU(s) list: 0-3
Thread(s) per core:  2
Core(s) per socket:  2
Socket(s):           1
NUMA node(s):        1
Vendor ID:           GenuineIntel
CPU family:          6
Model:               78
Model name:          Intel(R) Pentium(R) CPU 4405U @ 2.10GHz
Stepping:            3
CPU MHz:             500.010
CPU max MHz:         2100.0000
CPU min MHz:         400.0000
BogoMIPS:            4199.88
Virtualization:      VT-x
L1d cache:           32K
L1i cache:           32K
L2 cache:            256K
L3 cache:            2048K
NUMA node0 CPU(s):   0-3
Flags:               fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush dts acpi mmx fxsr sse sse2 ss ht tm pbe syscall nx pdpe1gb rdtscp lm constant_tsc art arch_perfmon pebs bts rep_good nopl xtopology nonstop_tsc cpuid aperfmperf pni pclmulqdq dtes64 monitor ds_cpl vmx est tm2 ssse3 sdbg cx16 xtpr pdcm pcid sse4_1 sse4_2 x2apic movbe popcnt tsc_deadline_timer aes xsave rdrand lahf_lm abm 3dnowprefetch cpuid_fault epb invpcid_single pti ssbd ibrs ibpb stibp tpr_shadow vnmi flexpriority ept vpid ept_ad fsgsbase tsc_adjust erms invpcid rdseed smap clflushopt intel_pt xsaveopt xsavec xgetbv1 xsaves dtherm ida arat pln pts hwp hwp_notify hwp_act_window hwp_epp md_clear flush_l1d
```

# 獲取硬碟和目錄大小

> df -h

```
Filesystem      Size  Used Avail Use% Mounted on
udev            3.8G     0  3.8G   0% /dev
tmpfs           782M  2.0M  781M   1% /run
/dev/sda2       219G   25G  183G  12% /
tmpfs           3.9G  385M  3.5G  10% /dev/shm
tmpfs           5.0M  4.0K  5.0M   1% /run/lock
tmpfs           3.9G     0  3.9G   0% /sys/fs/cgroup
/dev/loop0      2.3M  2.3M     0 100% /snap/gnome-system-monitor/148
/dev/loop1      3.8M  3.8M     0 100% /snap/gnome-system-monitor/127
/dev/loop2       58M   58M     0 100% /snap/discord/115
/dev/loop3       45M   45M     0 100% /snap/gtk-common-themes/1440
/dev/loop4      4.3M  4.3M     0 100% /snap/gnome-calculator/544
/dev/loop5      384K  384K     0 100% /snap/gnome-characters/570
/dev/loop6       56M   56M     0 100% /snap/core18/1932
/dev/loop7       63M   63M     0 100% /snap/gtk-common-themes/1506
/dev/loop8      163M  163M     0 100% /snap/gnome-3-28-1804/145
/dev/loop9      218M  218M     0 100% /snap/gnome-3-34-1804/60
/dev/loop11      15M   15M     0 100% /snap/gnome-characters/399
/dev/loop10     1.0M  1.0M     0 100% /snap/gnome-logs/81
/dev/loop12     162M  162M     0 100% /snap/gnome-3-28-1804/128
/dev/loop13      98M   98M     0 100% /snap/core/9993
/dev/loop14     2.5M  2.5M     0 100% /snap/gnome-calculator/826
/dev/loop15      98M   98M     0 100% /snap/core/10185
/dev/loop16     1.0M  1.0M     0 100% /snap/gnome-logs/100
/dev/loop17      56M   56M     0 100% /snap/core18/1885
/dev/sda1       511M  6.2M  505M   2% /boot/efi
tmpfs           782M   16K  782M   1% /run/user/121
tmpfs           782M   76K  782M   1% /run/user/1000
/dev/sdb1       932G  779G  154G  84% /media/xuan/TOSHIBA_XUAN
```

# 查詢 Linux 的發行版名稱與版本

> cat /etc/os-release

```
NAME="Ubuntu"
VERSION="18.04.5 LTS (Bionic Beaver)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 18.04.5 LTS"
VERSION_ID="18.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=bionic
UBUNTU_CODENAME=bionic
```

# 檢查系統內實體記憶體及 Swap 的使用情況

> free -h

```
              total        used        free      shared  buff/cache   available
Mem:           7.6G        3.1G        297M        911M        4.2G        3.4G
Swap:          2.0G        512K        2.0G
```
