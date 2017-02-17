Cloude provider : AWS
AMI CentOS 6-4 -x86_64- - Release Media-6-4
OS CentOS 6.4

Volumn space
```
[root@ip-172-31-7-27 ~]# df -aTh
Filesystem    Type    Size  Used Avail Use% Mounted on
/dev/xvde     ext4     69G  644M   65G   1% /
proc          proc       0     0     0   -  /proc
sysfs        sysfs       0     0     0   -  /sys
devpts      devpts       0     0     0   -  /dev/pts
tmpfs        tmpfs    7.4G     0  7.4G   0% /dev/shm
none   binfmt_misc       0     0     0   -  /proc/sys/fs/binfmt_misc
```

Repo list
```
[root@ip-172-31-7-27 ~]# yum repolist enabled
Loaded plugins: fastestmirror, presto
base                                                                                                                                                                                                                  | 3.7 kB     00:00
base/primary_db                                                                                                                                                                                                       | 4.7 MB     00:00
extras                                                                                                                                                                                                                | 3.4 kB     00:00
extras/primary_db                                                                                                                                                                                                     |  37 kB     00:00
updates                                                                                                                                                                                                               | 3.4 kB     00:00
updates/primary_db                                                                                                                                                                                                    | 4.3 MB     00:00
repo id                                                                                                       repo name                                                                                                                status
base                                                                                                          CentOS-6 - Base                                                                                                          6,696
extras                                                                                                        CentOS-6 - Extras                                                                                                           63
updates                                                                                                       CentOS-6 - Updates                                                                                                         825
repolist: 7,584
```

Linux users/group
```
[root@ip-172-31-7-41 ~]# cat /etc/passwd | grep raffles
raffles:x:2000:2000::/home/raffles:/bin/bash
[root@ip-172-31-7-41 ~]# cat /etc/passwd | grep fullerton
fullerton:x:3000:3000::/home/fullerton:/bin/bash
[root@ip-172-31-7-41 ~]# cat /etc/group | grep hotels
hotels:x:3001:fullerton
[root@ip-172-31-7-41 ~]# cat /etc/group | grep shops
shops:x:3002:raffles
```