```
mysql> show slave status \G;
*************************** 1. row ***************************
               Slave_IO_State: Waiting for master to send event
                  Master_Host: ip-172-31-14-10.ap-southeast-1.compute.internal
                  Master_User: root
                  Master_Port: 3306
                Connect_Retry: 60
              Master_Log_File: mysql-replication.000004
          Read_Master_Log_Pos: 3777
               Relay_Log_File: mysqld-relay-bin.000002
                Relay_Log_Pos: 706
        Relay_Master_Log_File: mysql-replication.000004
             Slave_IO_Running: Yes
            Slave_SQL_Running: No
              Replicate_Do_DB: replicadb
          Replicate_Ignore_DB:
           Replicate_Do_Table:
       Replicate_Ignore_Table:
      Replicate_Wild_Do_Table:
  Replicate_Wild_Ignore_Table:
                   Last_Errno: 1049
                   Last_Error: Error 'Unknown database 'replicadb'' on query. Default database: 'replicadb'. Query: 'create table test ( col1 integer)'
                 Skip_Counter: 0
          Exec_Master_Log_Pos: 918
              Relay_Log_Space: 3722
              Until_Condition: None
               Until_Log_File:
                Until_Log_Pos: 0
           Master_SSL_Allowed: No
           Master_SSL_CA_File:
           Master_SSL_CA_Path:
              Master_SSL_Cert:
            Master_SSL_Cipher:
               Master_SSL_Key:
        Seconds_Behind_Master: NULL
Master_SSL_Verify_Server_Cert: No
                Last_IO_Errno: 0
                Last_IO_Error:
               Last_SQL_Errno: 1049
               Last_SQL_Error: Error 'Unknown database 'replicadb'' on query. Default database: 'replicadb'. Query: 'create table test ( col1 integer)'
  Replicate_Ignore_Server_Ids:
             Master_Server_Id: 1
1 row in set (0.00 sec)
```
