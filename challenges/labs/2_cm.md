List repo
```
[root@ip-172-31-7-27 ~]# ls /etc/yum.repos.d
CentOS-Base.repo  CentOS-Debuginfo.repo  CentOS-fasttrack.repo  CentOS-Media.repo  CentOS-Vault.repo  cloudera-manager.repo  cloudera-manager.repo.~1~
```

Prepare DB command
```
/usr/share/cmf/schema/scm_prepare_database.sh mysql scm scm 1234 -h ip-172-31-1-16.ap-southeast-1.compute.internal
```