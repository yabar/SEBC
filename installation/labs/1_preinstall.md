Check vm.swappiness
```
[root@ip-172-31-14-10 vm]# cat /proc/sys/vm/swappiness
1
```

Show the mount attributes of all volumes
```
[root@ip-172-31-14-10 vm]# df -aTh
Filesystem    Type    Size  Used Avail Use% Mounted on
/dev/xvde     ext4    7.9G  635M  6.9G   9% /
proc          proc       0     0     0   -  /proc
sysfs        sysfs       0     0     0   -  /sys
devpts      devpts       0     0     0   -  /dev/pts
tmpfs        tmpfs    7.4G     0  7.4G   0% /dev/shm
none   binfmt_misc       0     0     0   -  /proc/sys/fs/binfmt_misc
```

Show the reserve space of any non-root, ext-based volumes
```
[root@ip-172-31-14-10 vm]# df -
Filesystem    Type    Size  Used Avail Use% Mounted on
/dev/xvde     ext4    7.9G  635M  6.9G   9% /
```

Disable transparent hugepages
```
[root@ip-172-31-14-10 mm]# cat /proc/sys/vm/nr_hugepages
0
[root@ip-172-31-14-10 mm]# cat /proc/sys/vm/nr_overcommit_hugepages
0
```


List your network interface configuration
```
[root@ip-172-31-14-10 mm]# ifconfig -a
eth0      Link encap:Ethernet  HWaddr 02:C6:6F:D7:D4:D3
          inet addr:172.31.14.10  Bcast:172.31.15.255  Mask:255.255.240.0
          inet6 addr: fe80::c6:6fff:fed7:d4d3/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:9001  Metric:1
          RX packets:2507 errors:0 dropped:0 overruns:0 frame:0
          TX packets:1641 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000
          RX bytes:170582 (166.5 KiB)  TX bytes:172803 (168.7 KiB)
          Interrupt:24

lo        Link encap:Local Loopback
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:16436  Metric:1
          RX packets:0 errors:0 dropped:0 overruns:0 frame:0
          TX packets:0 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0
          RX bytes:0 (0.0 b)  TX bytes:0 (0.0 b)
```


List forward and reverse host lookups 
```
[root@ip-172-31-14-10 mm]# getent ahostsv4 ec2-54-169-187-44.ap-southeast-1.compute.amazonaws.com
172.31.14.10    STREAM ec2-54-169-187-44.ap-southeast-1.compute.amazonaws.com
172.31.14.10    DGRAM
172.31.14.10    RAW
```

Show the nscd service is running
Show the ntpd service is running
```
[root@ip-172-31-14-10 etc]# service --status-all | grep nscd
[root@ip-172-31-14-10 etc]# service --status-all | grep ntpd
```
