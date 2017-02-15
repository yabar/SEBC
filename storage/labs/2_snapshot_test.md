```
[root@ip-172-31-14-10 ~]# hdfs dfs -mkdir /tmp/precious/
[root@ip-172-31-14-10 ~]# hdfs dfs -put /home/SEBC.zip /tmp/precious/
[root@ip-172-31-14-10 ~]# hdfs dfs -ls /tmp/precious/
Found 1 items
-rw-r--r--   3 root supergroup     414615 2017-02-15 07:44 /tmp/precious/SEBC.zip
[root@ip-172-31-14-10 ~]# hdfs dfsadmin -allowSnapshot /tmp/precious
Allowing snaphot on /tmp/precious succeeded
[root@ip-172-31-14-10 ~]# hdfs fs -createSnapshot /tmp/precious sebc_snap1
Error: Could not find or load main class fs
[root@ip-172-31-14-10 ~]# hdfs dfs -createSnapshot /tmp/precious sebc_snap1
Created snapshot /tmp/precious/.snapshot/sebc_snap1
[root@ip-172-31-14-10 ~]# hdfs dfs -createSnapshot /tmp/precious sebc-hdfs-test
Created snapshot /tmp/precious/.snapshot/sebc-hdfs-test
[root@ip-172-31-14-10 ~]# hdfs dfs -lsr /tmp/precious/.snapshot
lsr: DEPRECATED: Please use 'ls -R' instead.
drwxr-xr-x   - root supergroup          0 2017-02-15 07:48 /tmp/precious/.snapshot/sebc-hdfs-test
-rw-r--r--   3 root supergroup     414615 2017-02-15 07:44 /tmp/precious/.snapshot/sebc-hdfs-test/SEBC.zip
drwxr-xr-x   - root supergroup          0 2017-02-15 07:47 /tmp/precious/.snapshot/sebc_snap1
-rw-r--r--   3 root supergroup     414615 2017-02-15 07:44 /tmp/precious/.snapshot/sebc_snap1/SEBC.zip
[root@ip-172-31-14-10 ~]# hdfs dfs -rm /tmp/precious/SEBC.zip
17/02/15 07:50:52 INFO fs.TrashPolicyDefault: Moved: 'hdfs://nameservice1/tmp/precious/SEBC.zip' to trash at: hdfs://nameservice1/user/root/.Trash/Current/tmp/precious/SEBC.zip
[root@ip-172-31-14-10 ~]# hdfs dfs -cp -ptopax /tmp/precious/.snapshot/sebc-hdfs-test/SEBC.zip /tmp/precious
[root@ip-172-31-14-10 ~]# hdfs dfs -lsr /tmp/precious/
lsr: DEPRECATED: Please use 'ls -R' instead.
-rw-r--r--   3 root supergroup     414615 2017-02-15 07:44 /tmp/precious/SEBC.zip
```
