```
[root@ip-172-31-1-16 ~]# hostname -f
ip-172-31-1-16.ap-southeast-1.compute.internal
[root@ip-172-31-1-16 ~]# mysql --version
mysql  Ver 14.14 Distrib 5.5.54, for Linux (x86_64) using readline 5.1
[root@ip-172-31-1-16 ~]# mysql -u root -p -e 'show databases'
Enter password:
+--------------------+
| Database           |
+--------------------+
| information_schema |
| hive               |
| hue                |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
```

