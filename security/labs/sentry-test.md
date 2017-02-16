Senry test
```
[yabar@ip-172-31-14-10 ~]$ beeline
Beeline version 1.1.0-cdh5.8.4 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM
scan complete in 5ms
Connecting to jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM
Enter username for jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM: yabar
Enter password for jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM: ****
Connected to: Apache Hive (version 1.1.0-cdh5.8.4)
Driver: Hive JDBC (version 1.1.0-cdh5.8.4)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-14-10.ap-southeast-> show tables;
INFO  : Compiling command(queryId=hive_20170216094040_9d841ab8-b7fb-4968-b2d9-66dee448389d): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170216094040_9d841ab8-b7fb-4968-b2d9-66dee448389d); Time taken: 0.763 seconds
INFO  : Executing command(queryId=hive_20170216094040_9d841ab8-b7fb-4968-b2d9-66dee448389d): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170216094040_9d841ab8-b7fb-4968-b2d9-66dee448389d); Time taken: 0.291 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.413 seconds)
0: jdbc:hive2://ip-172-31-14-10.ap-southeast->
```


kinit as george --> show tables
```
[yabar@ip-172-31-14-10 ~]$ kdestroy
[yabar@ip-172-31-14-10 ~]$ kinit george
Password for george@YABAR.COM:
[yabar@ip-172-31-14-10 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_500
Default principal: george@YABAR.COM

Valid starting     Expires            Service principal
02/16/17 10:41:45  02/17/17 10:41:45  krbtgt/YABAR.COM@YABAR.COM
        renew until 02/23/17 10:41:45
[yabar@ip-172-31-14-10 ~]$ beeline
Beeline version 1.1.0-cdh5.8.4 by Apache Hive
beeline> [yabar@ip-172-31-14-10 ~]$ beeline
Beeline version 1.1.0-cdh5.8.4 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM
scan complete in 3ms
Connecting to jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM
Enter username for jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM: george
Enter password for jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM:
Connected to: Apache Hive (version 1.1.0-cdh5.8.4)
Driver: Hive JDBC (version 1.1.0-cdh5.8.4)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-14-10.ap-southeast-> show tables;
INFO  : Compiling command(queryId=hive_20170216104343_0a45df4b-5643-407d-b226-aa6e6188b2f5): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170216104343_0a45df4b-5643-407d-b226-aa6e6188b2f5); Time taken: 0.074 seconds
INFO  : Executing command(queryId=hive_20170216104343_0a45df4b-5643-407d-b226-aa6e6188b2f5): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170216104343_0a45df4b-5643-407d-b226-aa6e6188b2f5); Time taken: 0.137 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.354 seconds)
```

kinit as ferdinand --> show tables
```
[yabar@ip-172-31-14-10 ~]$ kdestroy
[yabar@ip-172-31-14-10 ~]$ kinit ferdinand
Password for ferdinand@YABAR.COM:
[yabar@ip-172-31-14-10 ~]$ beeline
Beeline version 1.1.0-cdh5.8.4 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM
scan complete in 3ms
Connecting to jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM
Enter username for jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM: ferdinand
Enter password for jdbc:hive2://ip-172-31-14-10.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-14-10.ap-southeast-1.compute.internal@YABAR.COM:
Connected to: Apache Hive (version 1.1.0-cdh5.8.4)
Driver: Hive JDBC (version 1.1.0-cdh5.8.4)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-14-10.ap-southeast-> show tables;
INFO  : Compiling command(queryId=hive_20170216104646_09c1947d-fe1a-416c-8081-ea771c1b439b): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170216104646_09c1947d-fe1a-416c-8081-ea771c1b439b); Time taken: 0.1 seconds
INFO  : Executing command(queryId=hive_20170216104646_09c1947d-fe1a-416c-8081-ea771c1b439b): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170216104646_09c1947d-fe1a-416c-8081-ea771c1b439b); Time taken: 0.141 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.38 seconds)
```
