
```
login as: ruffles
Server refused our key
ruffles@ec2-52-221-246-62.ap-southeast-1.compute.amazonaws.com's password:
Access denied
ruffles@ec2-52-221-246-62.ap-southeast-1.compute.amazonaws.com's password:
Access denied
ruffles@ec2-52-221-246-62.ap-southeast-1.compute.amazonaws.com's password:

────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────

Session stopped
    - Press <return> to exit tab
    - Press R to restart session
    - Press S to save terminal output to file
login as: raffles
Server refused our key
raffles@ec2-52-221-246-62.ap-southeast-1.compute.amazonaws.com's password:
     ┌────────────────────────────────────────────────────────────────────┐
     │                         • MobaXterm 9.4 •                          │
     │            (SSH client, X-server and networking tools)             │
     │                                                                    │
     │ ➤ SSH session to raffles@ec2-52-221-246-62.ap-southeast-1.compute.amazonaws.com│
     │   • SSH compression : ✔                                            │
     │   • SSH-browser     : ✔                                            │
     │   • X11-forwarding  : ✘  (disabled or not supported by server)     │
     │   • DISPLAY         : 10.2.6.169:0.0                               │
     │                                                                    │
     │ ➤ For more info, ctrl+click on help or visit our website           │
     └────────────────────────────────────────────────────────────────────┘

Last login: Fri Feb 17 07:08:08 2017 from 167.220.255.140
[raffles@ip-172-31-7-27 ~]$ hdfs dfs -chmod -R 771 /user/hive/warehouse
17/02/17 07:54:43 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:54:45 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:54:45 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318083272
17/02/17 07:54:46 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:54:46 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318083272
17/02/17 07:54:50 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:54:50 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318083272
^C^C^C^C^C^C^C17/02/17 07:54:54 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:54:54 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318083272
17/02/17 07:54:56 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:54:56 WARN ipc.Client: Couldn't setup connection for raffles@YABAR.SG to ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8020
javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:212)
        at org.apache.hadoop.security.SaslRpcClient.saslConnect(SaslRpcClient.java:413)
        at org.apache.hadoop.ipc.Client$Connection.setupSaslConnection(Client.java:561)
        at org.apache.hadoop.ipc.Client$Connection.access$1900(Client.java:376)
        at org.apache.hadoop.ipc.Client$Connection$2.run(Client.java:731)
        at org.apache.hadoop.ipc.Client$Connection$2.run(Client.java:727)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1796)
        at org.apache.hadoop.ipc.Client$Connection.setupIOstreams(Client.java:726)
        at org.apache.hadoop.ipc.Client$Connection.access$2900(Client.java:376)
        at org.apache.hadoop.ipc.Client.getConnection(Client.java:1525)
        at org.apache.hadoop.ipc.Client.call(Client.java:1448)
        at org.apache.hadoop.ipc.Client.call(Client.java:1409)
        at org.apache.hadoop.ipc.ProtobufRpcEngine$Invoker.invoke(ProtobufRpcEngine.java:230)
        at com.sun.proxy.$Proxy16.getFileInfo(Unknown Source)
        at org.apache.hadoop.hdfs.protocolPB.ClientNamenodeProtocolTranslatorPB.getFileInfo(ClientNamenodeProtocolTranslatorPB.java:771)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.io.retry.RetryInvocationHandler.invokeMethod(RetryInvocationHandler.java:256)
        at org.apache.hadoop.io.retry.RetryInvocationHandler.invoke(RetryInvocationHandler.java:104)
        at com.sun.proxy.$Proxy17.getFileInfo(Unknown Source)
        at org.apache.hadoop.hdfs.DFSClient.getFileInfo(DFSClient.java:2123)
        at org.apache.hadoop.hdfs.DistributedFileSystem$20.doCall(DistributedFileSystem.java:1253)
        at org.apache.hadoop.hdfs.DistributedFileSystem$20.doCall(DistributedFileSystem.java:1249)
        at org.apache.hadoop.fs.FileSystemLinkResolver.resolve(FileSystemLinkResolver.java:81)
        at org.apache.hadoop.hdfs.DistributedFileSystem.getFileStatus(DistributedFileSystem.java:1249)
        at org.apache.hadoop.fs.Globber.getFileStatus(Globber.java:64)
        at org.apache.hadoop.fs.Globber.doGlob(Globber.java:272)
        at org.apache.hadoop.fs.Globber.glob(Globber.java:151)
        at org.apache.hadoop.fs.FileSystem.globStatus(FileSystem.java:1703)
        at org.apache.hadoop.fs.shell.PathData.expandAsGlob(PathData.java:326)
        at org.apache.hadoop.fs.shell.Command.expandArgument(Command.java:235)
        at org.apache.hadoop.fs.shell.Command.expandArguments(Command.java:218)
        at org.apache.hadoop.fs.shell.FsCommand.processRawArguments(FsCommand.java:102)
        at org.apache.hadoop.fs.shell.Command.run(Command.java:165)
        at org.apache.hadoop.fs.FsShell.run(FsShell.java:315)
        at org.apache.hadoop.util.ToolRunner.run(ToolRunner.java:70)
        at org.apache.hadoop.util.ToolRunner.run(ToolRunner.java:84)
        at org.apache.hadoop.fs.FsShell.main(FsShell.java:372)
Caused by: GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:710)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:248)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:179)
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:193)
        ... 41 more
Caused by: KrbException: Generic error (description in e-text) (60) - PROCESS_TGS
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:73)
        at sun.security.krb5.KrbTgsReq.getReply(KrbTgsReq.java:192)
        at sun.security.krb5.KrbTgsReq.sendAndGetCreds(KrbTgsReq.java:203)
        at sun.security.krb5.internal.CredentialsUtil.serviceCreds(CredentialsUtil.java:309)
        at sun.security.krb5.internal.CredentialsUtil.acquireServiceCreds(CredentialsUtil.java:115)
        at sun.security.krb5.Credentials.acquireServiceCreds(Credentials.java:454)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:641)
        ... 44 more
Caused by: KrbException: Identifier doesn't match expected value (906)
        at sun.security.krb5.internal.KDCRep.init(KDCRep.java:143)
        at sun.security.krb5.internal.TGSRep.init(TGSRep.java:66)
        at sun.security.krb5.internal.TGSRep.<init>(TGSRep.java:61)
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:55)
        ... 50 more
17/02/17 07:54:56 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:java.io.IOException: Couldn't setup connection for raffles@YABAR.SG to ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8020
chmod: Failed on local exception: java.io.IOException: Couldn't setup connection for raffles@YABAR.SG to ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8020; Host Details : local host is: "ip-172-31-7-27.ap-southeast-1.compute.internal/172.31.7.27"; destination host is: "ip-172-31-1-16.ap-southeast-1.compute.internal":8020;
[raffles@ip-172-31-7-27 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_2000
Default principal: raffles@YABAR.SG

Valid starting     Expires            Service principal
02/17/17 07:08:18  02/18/17 07:08:18  krbtgt/YABAR.SG@YABAR.SG
        renew until 02/24/17 07:08:18
[raffles@ip-172-31-7-27 ~]$ hdfs dfs -ls /user/hive/warehouse
17/02/17 07:55:35 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:55:38 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:55:38 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318135465
^C^C^C^C^C^C^C17/02/17 07:55:41 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:55:41 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318135465
17/02/17 07:55:43 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:55:43 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318135465
17/02/17 07:55:44 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:55:44 WARN security.UserGroupInformation: Not attempting to re-login since the last re-login was attempted less than 60 seconds before. Last Login=1487318135465
17/02/17 07:55:46 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
17/02/17 07:55:46 WARN ipc.Client: Couldn't setup connection for raffles@YABAR.SG to ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8020
javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)]
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:212)
        at org.apache.hadoop.security.SaslRpcClient.saslConnect(SaslRpcClient.java:413)
        at org.apache.hadoop.ipc.Client$Connection.setupSaslConnection(Client.java:561)
        at org.apache.hadoop.ipc.Client$Connection.access$1900(Client.java:376)
        at org.apache.hadoop.ipc.Client$Connection$2.run(Client.java:731)
        at org.apache.hadoop.ipc.Client$Connection$2.run(Client.java:727)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1796)
        at org.apache.hadoop.ipc.Client$Connection.setupIOstreams(Client.java:726)
        at org.apache.hadoop.ipc.Client$Connection.access$2900(Client.java:376)
        at org.apache.hadoop.ipc.Client.getConnection(Client.java:1525)
        at org.apache.hadoop.ipc.Client.call(Client.java:1448)
        at org.apache.hadoop.ipc.Client.call(Client.java:1409)
        at org.apache.hadoop.ipc.ProtobufRpcEngine$Invoker.invoke(ProtobufRpcEngine.java:230)
        at com.sun.proxy.$Proxy16.getFileInfo(Unknown Source)
        at org.apache.hadoop.hdfs.protocolPB.ClientNamenodeProtocolTranslatorPB.getFileInfo(ClientNamenodeProtocolTranslatorPB.java:771)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.io.retry.RetryInvocationHandler.invokeMethod(RetryInvocationHandler.java:256)
        at org.apache.hadoop.io.retry.RetryInvocationHandler.invoke(RetryInvocationHandler.java:104)
        at com.sun.proxy.$Proxy17.getFileInfo(Unknown Source)
        at org.apache.hadoop.hdfs.DFSClient.getFileInfo(DFSClient.java:2123)
        at org.apache.hadoop.hdfs.DistributedFileSystem$20.doCall(DistributedFileSystem.java:1253)
        at org.apache.hadoop.hdfs.DistributedFileSystem$20.doCall(DistributedFileSystem.java:1249)
        at org.apache.hadoop.fs.FileSystemLinkResolver.resolve(FileSystemLinkResolver.java:81)
        at org.apache.hadoop.hdfs.DistributedFileSystem.getFileStatus(DistributedFileSystem.java:1249)
        at org.apache.hadoop.fs.Globber.getFileStatus(Globber.java:64)
        at org.apache.hadoop.fs.Globber.doGlob(Globber.java:272)
        at org.apache.hadoop.fs.Globber.glob(Globber.java:151)
        at org.apache.hadoop.fs.FileSystem.globStatus(FileSystem.java:1703)
        at org.apache.hadoop.fs.shell.PathData.expandAsGlob(PathData.java:326)
        at org.apache.hadoop.fs.shell.Command.expandArgument(Command.java:235)
        at org.apache.hadoop.fs.shell.Command.expandArguments(Command.java:218)
        at org.apache.hadoop.fs.shell.FsCommand.processRawArguments(FsCommand.java:102)
        at org.apache.hadoop.fs.shell.Command.run(Command.java:165)
        at org.apache.hadoop.fs.FsShell.run(FsShell.java:315)
        at org.apache.hadoop.util.ToolRunner.run(ToolRunner.java:70)
        at org.apache.hadoop.util.ToolRunner.run(ToolRunner.java:84)
        at org.apache.hadoop.fs.FsShell.main(FsShell.java:372)
Caused by: GSSException: No valid credentials provided (Mechanism level: Generic error (description in e-text) (60) - PROCESS_TGS)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:710)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:248)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:179)
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:193)
        ... 41 more
Caused by: KrbException: Generic error (description in e-text) (60) - PROCESS_TGS
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:73)
        at sun.security.krb5.KrbTgsReq.getReply(KrbTgsReq.java:192)
        at sun.security.krb5.KrbTgsReq.sendAndGetCreds(KrbTgsReq.java:203)
        at sun.security.krb5.internal.CredentialsUtil.serviceCreds(CredentialsUtil.java:309)
        at sun.security.krb5.internal.CredentialsUtil.acquireServiceCreds(CredentialsUtil.java:115)
        at sun.security.krb5.Credentials.acquireServiceCreds(Credentials.java:454)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:641)
        ... 44 more
Caused by: KrbException: Identifier doesn't match expected value (906)
        at sun.security.krb5.internal.KDCRep.init(KDCRep.java:143)
        at sun.security.krb5.internal.TGSRep.init(TGSRep.java:66)
        at sun.security.krb5.internal.TGSRep.<init>(TGSRep.java:61)
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:55)
        ... 50 more
17/02/17 07:55:46 WARN security.UserGroupInformation: PriviledgedActionException as:raffles@YABAR.SG (auth:KERBEROS) cause:java.io.IOException: Couldn't setup connection for raffles@YABAR.SG to ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8020
ls: Failed on local exception: java.io.IOException: Couldn't setup connection for raffles@YABAR.SG to ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8020; Host Details : local host is: "ip-172-31-7-27.ap-southeast-1.compute.internal/172.31.7.27"; destination host is: "ip-172-31-1-16.ap-southeast-1.compute.internal":8020;
[raffles@ip-172-31-7-27 ~]$ kdestroy
[raffles@ip-172-31-7-27 ~]$ kinit raffles@YABAR.SG
Password for raffles@YABAR.SG:
kinit: Password incorrect while getting initial credentials
[raffles@ip-172-31-7-27 ~]$ kinit raffles@YABAR.SG
Password for raffles@YABAR.SG:
[raffles@ip-172-31-7-27 ~]$ hdfs dfs -ls /user/hive/warehouse
Found 4 items
drwxrwxrwt   - yabar hive          0 2017-02-17 06:10 /user/hive/warehouse/customers
drwxrwxrwt   - yabar hive          0 2017-02-17 06:10 /user/hive/warehouse/sample_07
drwxrwxrwt   - yabar hive          0 2017-02-17 06:10 /user/hive/warehouse/sample_08
drwxrwxrwt   - yabar hive          0 2017-02-17 06:10 /user/hive/warehouse/web_logs
[raffles@ip-172-31-7-27 ~]$ hdfs dfs -chmod -R 771 /user/hive/warehouse
chmod: changing permissions of '/user/hive/warehouse': Permission denied. user=raffles is not the owner of inode=warehouse
[raffles@ip-172-31-7-27 ~]$ beeline
Beeline version 1.1.0-cdh5.10.0 by Apache Hive
beeline> exit
. . . .> ;
No current connection
beeline> hos[raffles@ip-172-31-7-27 ~]$ hostname -f
ip-172-31-7-27.ap-southeast-1.compute.internal
[raffles@ip-172-31-7-27 ~]$ beeline
Beeline version 1.1.0-cdh5.10.0 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-7-27.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-7-27.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
Could not open connection to the HS2 server. Please check the server URI and if the URI is correct, then ask the administrator to check the server status.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://ip-172-31-7-27.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM: java.net.ConnectException: Connection refused (state=08S01,code=0)
beeline> !connect jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
Connecting to jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
17/02/17 07:58:52 [main]: ERROR transport.TSaslTransport: SASL negotiation failure
javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)]
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:212)
        at org.apache.thrift.transport.TSaslClientTransport.handleSaslStartMessage(TSaslClientTransport.java:94)
        at org.apache.thrift.transport.TSaslTransport.open(TSaslTransport.java:271)
        at org.apache.thrift.transport.TSaslClientTransport.open(TSaslClientTransport.java:37)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:52)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:49)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1796)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport.open(TUGIAssumingTransport.java:49)
        at org.apache.hive.jdbc.HiveConnection.openTransport(HiveConnection.java:202)
        at org.apache.hive.jdbc.HiveConnection.<init>(HiveConnection.java:167)
        at org.apache.hive.jdbc.HiveDriver.connect(HiveDriver.java:105)
        at java.sql.DriverManager.getConnection(DriverManager.java:571)
        at java.sql.DriverManager.getConnection(DriverManager.java:187)
        at org.apache.hive.beeline.DatabaseConnection.connect(DatabaseConnection.java:146)
        at org.apache.hive.beeline.DatabaseConnection.getConnection(DatabaseConnection.java:211)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1467)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1362)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hive.beeline.ReflectiveCommandHandler.execute(ReflectiveCommandHandler.java:52)
        at org.apache.hive.beeline.BeeLine.execCommandWithPrefix(BeeLine.java:1131)
        at org.apache.hive.beeline.BeeLine.dispatch(BeeLine.java:1170)
        at org.apache.hive.beeline.BeeLine.execute(BeeLine.java:1003)
        at org.apache.hive.beeline.BeeLine.begin(BeeLine.java:915)
        at org.apache.hive.beeline.BeeLine.mainWithInputRedirection(BeeLine.java:511)
        at org.apache.hive.beeline.BeeLine.main(BeeLine.java:494)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.RunJar.run(RunJar.java:221)
        at org.apache.hadoop.util.RunJar.main(RunJar.java:136)
Caused by: GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:710)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:248)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:179)
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:193)
        ... 35 more
Caused by: KrbException: Server not found in Kerberos database (7) - UNKNOWN_SERVER
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:73)
        at sun.security.krb5.KrbTgsReq.getReply(KrbTgsReq.java:192)
        at sun.security.krb5.KrbTgsReq.sendAndGetCreds(KrbTgsReq.java:203)
        at sun.security.krb5.internal.CredentialsUtil.serviceCreds(CredentialsUtil.java:309)
        at sun.security.krb5.internal.CredentialsUtil.acquireServiceCreds(CredentialsUtil.java:115)
        at sun.security.krb5.Credentials.acquireServiceCreds(Credentials.java:454)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:641)
        ... 38 more
Caused by: KrbException: Identifier doesn't match expected value (906)
        at sun.security.krb5.internal.KDCRep.init(KDCRep.java:143)
        at sun.security.krb5.internal.TGSRep.init(TGSRep.java:66)
        at sun.security.krb5.internal.TGSRep.<init>(TGSRep.java:61)
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:55)
        ... 44 more
Unknown HS2 problem when communicating with Thrift server.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM: GSS initiate failed (state=08S01,code=0)
beeline> !connect jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
Connecting to jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
17/02/17 08:02:12 [main]: ERROR transport.TSaslTransport: SASL negotiation failure
javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)]
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:212)
        at org.apache.thrift.transport.TSaslClientTransport.handleSaslStartMessage(TSaslClientTransport.java:94)
        at org.apache.thrift.transport.TSaslTransport.open(TSaslTransport.java:271)
        at org.apache.thrift.transport.TSaslClientTransport.open(TSaslClientTransport.java:37)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:52)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:49)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1796)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport.open(TUGIAssumingTransport.java:49)
        at org.apache.hive.jdbc.HiveConnection.openTransport(HiveConnection.java:202)
        at org.apache.hive.jdbc.HiveConnection.<init>(HiveConnection.java:167)
        at org.apache.hive.jdbc.HiveDriver.connect(HiveDriver.java:105)
        at java.sql.DriverManager.getConnection(DriverManager.java:571)
        at java.sql.DriverManager.getConnection(DriverManager.java:187)
        at org.apache.hive.beeline.DatabaseConnection.connect(DatabaseConnection.java:146)
        at org.apache.hive.beeline.DatabaseConnection.getConnection(DatabaseConnection.java:211)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1467)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1362)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hive.beeline.ReflectiveCommandHandler.execute(ReflectiveCommandHandler.java:52)
        at org.apache.hive.beeline.BeeLine.execCommandWithPrefix(BeeLine.java:1131)
        at org.apache.hive.beeline.BeeLine.dispatch(BeeLine.java:1170)
        at org.apache.hive.beeline.BeeLine.execute(BeeLine.java:1003)
        at org.apache.hive.beeline.BeeLine.begin(BeeLine.java:915)
        at org.apache.hive.beeline.BeeLine.mainWithInputRedirection(BeeLine.java:511)
        at org.apache.hive.beeline.BeeLine.main(BeeLine.java:494)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.RunJar.run(RunJar.java:221)
        at org.apache.hadoop.util.RunJar.main(RunJar.java:136)
Caused by: GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:710)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:248)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:179)
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:193)
        ... 35 more
Caused by: KrbException: Server not found in Kerberos database (7) - UNKNOWN_SERVER
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:73)
        at sun.security.krb5.KrbTgsReq.getReply(KrbTgsReq.java:192)
        at sun.security.krb5.KrbTgsReq.sendAndGetCreds(KrbTgsReq.java:203)
        at sun.security.krb5.internal.CredentialsUtil.serviceCreds(CredentialsUtil.java:309)
        at sun.security.krb5.internal.CredentialsUtil.acquireServiceCreds(CredentialsUtil.java:115)
        at sun.security.krb5.Credentials.acquireServiceCreds(Credentials.java:454)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:641)
        ... 38 more
Caused by: KrbException: Identifier doesn't match expected value (906)
        at sun.security.krb5.internal.KDCRep.init(KDCRep.java:143)
        at sun.security.krb5.internal.TGSRep.init(TGSRep.java:66)
        at sun.security.krb5.internal.TGSRep.<init>(TGSRep.java:61)
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:55)
        ... 44 more
Unknown HS2 problem when communicating with Thrift server.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM: GSS initiate failed (state=08S01,code=0)
beeline> !connect jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
Connecting to jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
17/02/17 08:02:15 [main]: ERROR transport.TSaslTransport: SASL negotiation failure
javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)]
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:212)
        at org.apache.thrift.transport.TSaslClientTransport.handleSaslStartMessage(TSaslClientTransport.java:94)
        at org.apache.thrift.transport.TSaslTransport.open(TSaslTransport.java:271)
        at org.apache.thrift.transport.TSaslClientTransport.open(TSaslClientTransport.java:37)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:52)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:49)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1796)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport.open(TUGIAssumingTransport.java:49)
        at org.apache.hive.jdbc.HiveConnection.openTransport(HiveConnection.java:202)
        at org.apache.hive.jdbc.HiveConnection.<init>(HiveConnection.java:167)
        at org.apache.hive.jdbc.HiveDriver.connect(HiveDriver.java:105)
        at java.sql.DriverManager.getConnection(DriverManager.java:571)
        at java.sql.DriverManager.getConnection(DriverManager.java:187)
        at org.apache.hive.beeline.DatabaseConnection.connect(DatabaseConnection.java:146)
        at org.apache.hive.beeline.DatabaseConnection.getConnection(DatabaseConnection.java:211)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1467)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1362)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hive.beeline.ReflectiveCommandHandler.execute(ReflectiveCommandHandler.java:52)
        at org.apache.hive.beeline.BeeLine.execCommandWithPrefix(BeeLine.java:1131)
        at org.apache.hive.beeline.BeeLine.dispatch(BeeLine.java:1170)
        at org.apache.hive.beeline.BeeLine.execute(BeeLine.java:1003)
        at org.apache.hive.beeline.BeeLine.begin(BeeLine.java:915)
        at org.apache.hive.beeline.BeeLine.mainWithInputRedirection(BeeLine.java:511)
        at org.apache.hive.beeline.BeeLine.main(BeeLine.java:494)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.RunJar.run(RunJar.java:221)
        at org.apache.hadoop.util.RunJar.main(RunJar.java:136)
Caused by: GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:710)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:248)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:179)
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:193)
        ... 35 more
Caused by: KrbException: Server not found in Kerberos database (7) - UNKNOWN_SERVER
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:73)
        at sun.security.krb5.KrbTgsReq.getReply(KrbTgsReq.java:192)
        at sun.security.krb5.KrbTgsReq.sendAndGetCreds(KrbTgsReq.java:203)
        at sun.security.krb5.internal.CredentialsUtil.serviceCreds(CredentialsUtil.java:309)
        at sun.security.krb5.internal.CredentialsUtil.acquireServiceCreds(CredentialsUtil.java:115)
        at sun.security.krb5.Credentials.acquireServiceCreds(Credentials.java:454)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:641)
        ... 38 more
Caused by: KrbException: Identifier doesn't match expected value (906)
        at sun.security.krb5.internal.KDCRep.init(KDCRep.java:143)
        at sun.security.krb5.internal.TGSRep.init(TGSRep.java:66)
        at sun.security.krb5.internal.TGSRep.<init>(TGSRep.java:61)
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:55)
        ... 44 more
Unknown HS2 problem when communicating with Thrift server.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM: GSS initiate failed (state=08S01,code=0)
beeline> !connect jdbc:hive2://ip-172-31-7-27.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
Connecting to jdbc:hive2://ip-172-31-7-27.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
Could not open connection to the HS2 server. Please check the server URI and if the URI is correct, then ask the administrator to check the server status.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://ip-172-31-7-27.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM: java.net.ConnectException: Connection refused (state=08S01,code=0)
beeline> !connect jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
Connecting to jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM
17/02/17 08:02:20 [main]: ERROR transport.TSaslTransport: SASL negotiation failure
javax.security.sasl.SaslException: GSS initiate failed [Caused by GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)]
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:212)
        at org.apache.thrift.transport.TSaslClientTransport.handleSaslStartMessage(TSaslClientTransport.java:94)
        at org.apache.thrift.transport.TSaslTransport.open(TSaslTransport.java:271)
        at org.apache.thrift.transport.TSaslClientTransport.open(TSaslClientTransport.java:37)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:52)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport$1.run(TUGIAssumingTransport.java:49)
        at java.security.AccessController.doPrivileged(Native Method)
        at javax.security.auth.Subject.doAs(Subject.java:415)
        at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1796)
        at org.apache.hadoop.hive.thrift.client.TUGIAssumingTransport.open(TUGIAssumingTransport.java:49)
        at org.apache.hive.jdbc.HiveConnection.openTransport(HiveConnection.java:202)
        at org.apache.hive.jdbc.HiveConnection.<init>(HiveConnection.java:167)
        at org.apache.hive.jdbc.HiveDriver.connect(HiveDriver.java:105)
        at java.sql.DriverManager.getConnection(DriverManager.java:571)
        at java.sql.DriverManager.getConnection(DriverManager.java:187)
        at org.apache.hive.beeline.DatabaseConnection.connect(DatabaseConnection.java:146)
        at org.apache.hive.beeline.DatabaseConnection.getConnection(DatabaseConnection.java:211)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1467)
        at org.apache.hive.beeline.Commands.connect(Commands.java:1362)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hive.beeline.ReflectiveCommandHandler.execute(ReflectiveCommandHandler.java:52)
        at org.apache.hive.beeline.BeeLine.execCommandWithPrefix(BeeLine.java:1131)
        at org.apache.hive.beeline.BeeLine.dispatch(BeeLine.java:1170)
        at org.apache.hive.beeline.BeeLine.execute(BeeLine.java:1003)
        at org.apache.hive.beeline.BeeLine.begin(BeeLine.java:915)
        at org.apache.hive.beeline.BeeLine.mainWithInputRedirection(BeeLine.java:511)
        at org.apache.hive.beeline.BeeLine.main(BeeLine.java:494)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.RunJar.run(RunJar.java:221)
        at org.apache.hadoop.util.RunJar.main(RunJar.java:136)
Caused by: GSSException: No valid credentials provided (Mechanism level: Server not found in Kerberos database (7) - UNKNOWN_SERVER)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:710)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:248)
        at sun.security.jgss.GSSContextImpl.initSecContext(GSSContextImpl.java:179)
        at com.sun.security.sasl.gsskerb.GssKrb5Client.evaluateChallenge(GssKrb5Client.java:193)
        ... 35 more
Caused by: KrbException: Server not found in Kerberos database (7) - UNKNOWN_SERVER
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:73)
        at sun.security.krb5.KrbTgsReq.getReply(KrbTgsReq.java:192)
        at sun.security.krb5.KrbTgsReq.sendAndGetCreds(KrbTgsReq.java:203)
        at sun.security.krb5.internal.CredentialsUtil.serviceCreds(CredentialsUtil.java:309)
        at sun.security.krb5.internal.CredentialsUtil.acquireServiceCreds(CredentialsUtil.java:115)
        at sun.security.krb5.Credentials.acquireServiceCreds(Credentials.java:454)
        at sun.security.jgss.krb5.Krb5Context.initSecContext(Krb5Context.java:641)
        ... 38 more
Caused by: KrbException: Identifier doesn't match expected value (906)
        at sun.security.krb5.internal.KDCRep.init(KDCRep.java:143)
        at sun.security.krb5.internal.TGSRep.init(TGSRep.java:66)
        at sun.security.krb5.internal.TGSRep.<init>(TGSRep.java:61)
        at sun.security.krb5.KrbTgsRep.<init>(KrbTgsRep.java:55)
        ... 44 more
Unknown HS2 problem when communicating with Thrift server.
Error: Could not open client transport with JDBC Uri: jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-7-27.ap-southeast-1.compute.internal@YABAR.COM: GSS initiate failed (state=08S01,code=0)
beeline> [raffles@ip-172-31-7-27 ~]$
[raffles@ip-172-31-7-27 ~]$
[raffles@ip-172-31-7-27 ~]$
[raffles@ip-172-31-7-27 ~]$
[raffles@ip-172-31-7-27 ~]$ ls
[raffles@ip-172-31-7-27 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_2000
Default principal: raffles@YABAR.SG

Valid starting     Expires            Service principal
02/17/17 07:56:17  02/18/17 07:56:17  krbtgt/YABAR.SG@YABAR.SG
        renew until 02/24/17 07:56:17
[raffles@ip-172-31-7-27 ~]$ beeline
Beeline version 1.1.0-cdh5.10.0 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-1-16.ap-southeast-1.compute.internal@YABAR.COM
scan complete in 2ms
Connecting to jdbc:hive2://ip-172-31-1-16.ap-southeast-1.compute.internal:10000/default;principal=hive/ip-172-31-1-16.ap-southeast-1.compute.internal@YABAR.COM
Connected to: Apache Hive (version 1.1.0-cdh5.10.0)
Driver: Hive JDBC (version 1.1.0-cdh5.10.0)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> CREATE ROLE retail;
INFO  : Compiling command(queryId=hive_20170217080404_4504660d-0fc3-49a1-b7a3-71e7cf7303c9): CREATE ROLE retail
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_4504660d-0fc3-49a1-b7a3-71e7cf7303c9); Time taken: 0.574 seconds
INFO  : Executing command(queryId=hive_20170217080404_4504660d-0fc3-49a1-b7a3-71e7cf7303c9): CREATE ROLE retail
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_4504660d-0fc3-49a1-b7a3-71e7cf7303c9); Time taken: 0.973 seconds
INFO  : OK
No rows affected (2.896 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> GRANT SELECT ON DATABASE default TO ROLE retail;
INFO  : Compiling command(queryId=hive_20170217080404_41803dc7-7b67-47f5-8a9d-09befaa8e7ca): GRANT SELECT ON DATABASE default TO ROLE retail
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_41803dc7-7b67-47f5-8a9d-09befaa8e7ca); Time taken: 0.081 seconds
INFO  : Executing command(queryId=hive_20170217080404_41803dc7-7b67-47f5-8a9d-09befaa8e7ca): GRANT SELECT ON DATABASE default TO ROLE retail
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_41803dc7-7b67-47f5-8a9d-09befaa8e7ca); Time taken: 0.112 seconds
INFO  : OK
No rows affected (0.215 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> GRANT ROLE retail TO GROUP shops;
INFO  : Compiling command(queryId=hive_20170217080404_7bb1c190-052a-4627-9909-2988a9c3dc73): GRANT ROLE retail TO GROUP shops
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_7bb1c190-052a-4627-9909-2988a9c3dc73); Time taken: 0.068 seconds
INFO  : Executing command(queryId=hive_20170217080404_7bb1c190-052a-4627-9909-2988a9c3dc73): GRANT ROLE retail TO GROUP shops
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_7bb1c190-052a-4627-9909-2988a9c3dc73); Time taken: 0.078 seconds
INFO  : OK
No rows affected (0.162 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> GRANT SELECT ON DATABASE default TO ROLE retail;
INFO  : Compiling command(queryId=hive_20170217080404_8bd892f8-672b-4848-96ac-9390f5bb82fd): GRANT SELECT ON DATABASE default TO ROLE retail
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_8bd892f8-672b-4848-96ac-9390f5bb82fd); Time taken: 0.059 seconds
INFO  : Executing command(queryId=hive_20170217080404_8bd892f8-672b-4848-96ac-9390f5bb82fd): GRANT SELECT ON DATABASE default TO ROLE retail
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_8bd892f8-672b-4848-96ac-9390f5bb82fd); Time taken: 0.027 seconds
INFO  : OK
No rows affected (0.1 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> GRANT ROLE retail TO GROUP shops;
INFO  : Compiling command(queryId=hive_20170217080404_f8f51d43-e9a5-4060-b058-779f5327a21a): GRANT ROLE retail TO GROUP shops
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_f8f51d43-e9a5-4060-b058-779f5327a21a); Time taken: 0.087 seconds
INFO  : Executing command(queryId=hive_20170217080404_f8f51d43-e9a5-4060-b058-779f5327a21a): GRANT ROLE retail TO GROUP shops
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_f8f51d43-e9a5-4060-b058-779f5327a21a); Time taken: 0.029 seconds
INFO  : OK
No rows affected (0.132 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> CREATE ROLE hospitality
. . . . . . . . . . . . . . . . . . . . . . .> ;
INFO  : Compiling command(queryId=hive_20170217080404_a0086716-7848-42b9-9d9d-afe7dcc052b9): CREATE ROLE hospitality
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_a0086716-7848-42b9-9d9d-afe7dcc052b9); Time taken: 0.068 seconds
INFO  : Executing command(queryId=hive_20170217080404_a0086716-7848-42b9-9d9d-afe7dcc052b9): CREATE ROLE hospitality
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_a0086716-7848-42b9-9d9d-afe7dcc052b9); Time taken: 0.048 seconds
INFO  : OK
No rows affected (0.133 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> REVOKE ALL ON DATABASE default FROM ROLE hospitality;
INFO  : Compiling command(queryId=hive_20170217080404_a8524c98-bc9e-4993-a818-0903fbd0f847): REVOKE ALL ON DATABASE default FROM ROLE hospitality
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_a8524c98-bc9e-4993-a818-0903fbd0f847); Time taken: 0.062 seconds
INFO  : Executing command(queryId=hive_20170217080404_a8524c98-bc9e-4993-a818-0903fbd0f847): REVOKE ALL ON DATABASE default FROM ROLE hospitality
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_a8524c98-bc9e-4993-a818-0903fbd0f847); Time taken: 0.091 seconds
INFO  : OK
No rows affected (0.167 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> GRANT SELECT ON default.sample_07 TO ROLE hospitality;
INFO  : Compiling command(queryId=hive_20170217080404_b9e2fa31-fa71-4dbb-9346-40cb6258a352): GRANT SELECT ON default.sample_07 TO ROLE hospitality
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_b9e2fa31-fa71-4dbb-9346-40cb6258a352); Time taken: 0.059 seconds
INFO  : Executing command(queryId=hive_20170217080404_b9e2fa31-fa71-4dbb-9346-40cb6258a352): GRANT SELECT ON default.sample_07 TO ROLE hospitality
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_b9e2fa31-fa71-4dbb-9346-40cb6258a352); Time taken: 0.048 seconds
INFO  : OK
No rows affected (0.123 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> GRANT ROLE hospitality TO GROUP hotels;
INFO  : Compiling command(queryId=hive_20170217080404_4d677697-c629-44a3-ad33-af02bdcb3f29): GRANT ROLE hospitality TO GROUP hotels
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_4d677697-c629-44a3-ad33-af02bdcb3f29); Time taken: 0.065 seconds
INFO  : Executing command(queryId=hive_20170217080404_4d677697-c629-44a3-ad33-af02bdcb3f29): GRANT ROLE hospitality TO GROUP hotels
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_4d677697-c629-44a3-ad33-af02bdcb3f29); Time taken: 0.04 seconds
INFO  : OK
No rows affected (0.121 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> show tables;
INFO  : Compiling command(queryId=hive_20170217080404_55102d66-f509-441c-a8fd-5b7f81c481e3): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170217080404_55102d66-f509-441c-a8fd-5b7f81c481e3); Time taken: 0.224 seconds
INFO  : Executing command(queryId=hive_20170217080404_55102d66-f509-441c-a8fd-5b7f81c481e3): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170217080404_55102d66-f509-441c-a8fd-5b7f81c481e3); Time taken: 0.261 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
4 rows selected (0.624 seconds)
0: jdbc:hive2://ip-172-31-1-16.ap-southeast-1> DD

```