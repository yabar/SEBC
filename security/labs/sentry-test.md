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
