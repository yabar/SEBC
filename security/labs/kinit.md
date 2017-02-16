kinit
```
[yabar@ip-172-31-14-10 ~]$ kinit yabar/admin@YABAR.COM
Password for yabar/admin@YABAR.COM:
```

klist
```
[yabar@ip-172-31-14-10 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_500
Default principal: yabar/admin@YABAR.COM

Valid starting     Expires            Service principal
02/16/17 08:37:52  02/17/17 08:37:52  krbtgt/YABAR.COM@YABAR.COM
        renew until 02/23/17 08:37:52
```

Try HDFS
```
[yabar@ip-172-31-14-10 ~]$ hdfs dfs -ls /
Found 4 items
-rwxrwxrwx   3 hdfs supergroup       2058 2017-02-15 02:07 /passwd
drwxr-xr-x   - root supergroup          0 2017-02-15 08:57 /test
drwxrwxrwx   - hdfs supergroup          0 2017-02-16 08:06 /tmp
drwxr-xr-x   - hdfs supergroup          0 2017-02-15 07:01 /user
```
