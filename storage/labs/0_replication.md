Execute
```
hadoop distcp hdfs://54.254.160.237:8020/tmp/screenthong/source /tmp/yabar/ 
```

Error log from job history
```
2017-02-15 09:07:04,508 INFO [AsyncDispatcher event handler] org.apache.hadoop.mapreduce.v2.app.job.impl.TaskAttemptImpl: attempt_1487129473337_0012_m_000002_0 TaskAttempt Transitioned from RUNNING to FAIL_FINISHING_CONTAINER
2017-02-15 09:07:04,509 INFO [Thread-53] org.apache.hadoop.mapreduce.v2.app.rm.RMContainerRequestor: 1 failures on node ip-172-31-6-162.ap-southeast-1.compute.internal
2017-02-15 09:07:04,510 INFO [AsyncDispatcher event handler] org.apache.hadoop.mapreduce.v2.app.job.impl.TaskAttemptImpl: attempt_1487129473337_0012_m_000002_1 TaskAttempt Transitioned from NEW to UNASSIGNED
2017-02-15 09:07:04,510 INFO [Thread-53] org.apache.hadoop.mapreduce.v2.app.rm.RMContainerAllocator: Added attempt_1487129473337_0012_m_000002_1 to list of failed maps
2017-02-15 09:07:04,785 INFO [IPC Server handler 14 on 34489] org.apache.hadoop.mapred.TaskAttemptListenerImpl: Progress of TaskAttempt attempt_1487129473337_0012_m_000001_0 is : 1.0
2017-02-15 09:07:04,792 FATAL [IPC Server handler 15 on 34489] org.apache.hadoop.mapred.TaskAttemptListenerImpl: Task: attempt_1487129473337_0012_m_000001_0 - exited : java.io.IOException: File copy failed: hdfs://54.254.160.237:8020/tmp/screenthong/source/part-m-00000 --> hdfs://nameservice1/tmp/yabar/source/part-m-00000
	at org.apache.hadoop.tools.mapred.CopyMapper.copyFileWithRetry(CopyMapper.java:284)
	at org.apache.hadoop.tools.mapred.CopyMapper.map(CopyMapper.java:252)
	at org.apache.hadoop.tools.mapred.CopyMapper.map(CopyMapper.java:50)
	at org.apache.hadoop.mapreduce.Mapper.run(Mapper.java:145)
	at org.apache.hadoop.mapred.MapTask.runNewMapper(MapTask.java:787)
	at org.apache.hadoop.mapred.MapTask.run(MapTask.java:341)
	at org.apache.hadoop.mapred.YarnChild$2.run(YarnChild.java:164)
	at java.security.AccessController.doPrivileged(Native Method)
	at javax.security.auth.Subject.doAs(Subject.java:415)
	at org.apache.hadoop.security.UserGroupInformation.doAs(UserGroupInformation.java:1783)
	at org.apache.hadoop.mapred.YarnChild.main(YarnChild.java:158)
Caused by: java.io.IOException: Couldn't run retriable-command: Copying hdfs://54.254.160.237:8020/tmp/screenthong/source/part-m-00000 to hdfs://nameservice1/tmp/yabar/source/part-m-00000
	at org.apache.hadoop.tools.util.RetriableCommand.execute(RetriableCommand.java:101)
	at org.apache.hadoop.tools.mapred.CopyMapper.copyFileWithRetry(CopyMapper.java:280)
	... 10 more
Caused by: org.apache.hadoop.tools.mapred.RetriableFileCopyCommand$CopyReadException: org.apache.hadoop.hdfs.BlockMissingException: Could not obtain block: BP-106581566-172.31.8.59-1487053970381:blk_1073742716_1892 file=/tmp/screenthong/source/part-m-00000
	at org.apache.hadoop.tools.mapred.RetriableFileCopyCommand.readBytes(RetriableFileCopyCommand.java:291)
	at org.apache.hadoop.tools.mapred.RetriableFileCopyCommand.copyBytes(RetriableFileCopyCommand.java:251)
	at org.apache.hadoop.tools.mapred.RetriableFileCopyCommand.copyToFile(RetriableFileCopyCommand.java:184)
	at org.apache.hadoop.tools.mapred.RetriableFileCopyCommand.doCopy(RetriableFileCopyCommand.java:124)
	at org.apache.hadoop.tools.mapred.RetriableFileCopyCommand.doExecute(RetriableFileCopyCommand.java:100)
	at org.apache.hadoop.tools.util.RetriableCommand.execute(RetriableCommand.java:87)
	... 11 more
Caused by: org.apache.hadoop.hdfs.BlockMissingException: Could not obtain block: BP-106581566-172.31.8.59-1487053970381:blk_1073742716_1892 file=/tmp/screenthong/source/part-m-00000
	at org.apache.hadoop.hdfs.DFSInputStream.chooseDataNode(DFSInputStream.java:1001)
	at org.apache.hadoop.hdfs.DFSInputStream.blockSeekTo(DFSInputStream.java:648)
	at org.apache.hadoop.hdfs.DFSInputStream.readWithStrategy(DFSInputStream.java:889)
	at org.apache.hadoop.hdfs.DFSInputStream.read(DFSInputStream.java:942)
	at java.io.DataInputStream.read(DataInputStream.java:100)
	at org.apache.hadoop.tools.util.ThrottledInputStream.read(ThrottledInputStream.java:77)
	at org.apache.hadoop.tools.mapred.RetriableFileCopyCommand.readBytes(RetriableFileCopyCommand.java:286)
	... 16 more
```

Checked
- Lots of free space
- Can ping to the other Namenode using public IP
- Can do LS on the other HDFS using public IP
- Both removed firewall and security rule is set to All traffic all IP/Port
- Local put/get file to HDFS work fine
- Able to do local map reduce
- Restart each node
- Set private IP --> public IP on /etc/hosts  on both cluster
- `Could not obtain block: BP-106581566-172.31.8.59-1487053970381:blk_1073742716_1892 file=/tmp/screenthong/source/part-m-00000`
  This may be the problem; it tried to pick up blocks from a datanode with private IP, which doesn't work.

