[fullerton@ip-172-31-7-27 ~]$ kinit fullerton
Password for fullerton@YABAR.SG:
[fullerton@ip-172-31-7-27 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_3000
Default principal: fullerton@YABAR.SG

Valid starting     Expires            Service principal
02/17/17 07:20:22  02/18/17 07:20:22  krbtgt/YABAR.SG@YABAR.SG
        renew until 02/24/17 07:20:22
[fullerton@ip-172-31-7-27 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar pi 16 1000
Number of Maps  = 16
Samples per Map = 1000
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Wrote input for Map #8
Wrote input for Map #9
Wrote input for Map #10
Wrote input for Map #11
Wrote input for Map #12
Wrote input for Map #13
Wrote input for Map #14
Wrote input for Map #15
Starting Job
17/02/17 07:21:54 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8032
17/02/17 07:21:54 INFO input.FileInputFormat: Total input paths to process : 16
17/02/17 07:21:54 INFO mapreduce.JobSubmitter: number of splits:16
17/02/17 07:21:54 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1487311167324_0005
17/02/17 07:21:55 INFO impl.YarnClientImpl: Submitted application application_1487311167324_0005
17/02/17 07:21:55 INFO mapreduce.Job: The url to track the job: http://ip-172-31-1-16.ap-southeast-1.compute.internal:8088/proxy/application_1487311167324_0005/
17/02/17 07:21:55 INFO mapreduce.Job: Running job: job_1487311167324_0005
17/02/17 07:22:01 INFO mapreduce.Job: Job job_1487311167324_0005 running in uber mode : false
17/02/17 07:22:01 INFO mapreduce.Job:  map 0% reduce 0%
17/02/17 07:22:08 INFO mapreduce.Job:  map 6% reduce 0%
17/02/17 07:22:09 INFO mapreduce.Job:  map 13% reduce 0%
17/02/17 07:22:10 INFO mapreduce.Job:  map 31% reduce 0%
17/02/17 07:22:12 INFO mapreduce.Job:  map 75% reduce 0%
17/02/17 07:22:13 INFO mapreduce.Job:  map 81% reduce 0%
17/02/17 07:22:15 INFO mapreduce.Job:  map 94% reduce 0%
17/02/17 07:22:16 INFO mapreduce.Job:  map 100% reduce 0%
17/02/17 07:22:20 INFO mapreduce.Job:  map 100% reduce 100%
17/02/17 07:22:20 INFO mapreduce.Job: Job job_1487311167324_0005 completed successfully
17/02/17 07:22:20 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=132
                FILE: Number of bytes written=2134705
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=4902
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=67
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=16
                Launched reduce tasks=1
                Data-local map tasks=16
                Total time spent by all maps in occupied slots (ms)=119229
                Total time spent by all reduces in occupied slots (ms)=3739
                Total time spent by all map tasks (ms)=119229
                Total time spent by all reduce tasks (ms)=3739
                Total vcore-seconds taken by all map tasks=119229
                Total vcore-seconds taken by all reduce tasks=3739
                Total megabyte-seconds taken by all map tasks=122090496
                Total megabyte-seconds taken by all reduce tasks=3828736
        Map-Reduce Framework
                Map input records=16
                Map output records=32
                Map output bytes=288
                Map output materialized bytes=544
                Input split bytes=3014
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=544
                Reduce input records=32
                Reduce output records=0
                Spilled Records=64
                Shuffled Maps =16
                Failed Shuffles=0
                Merged Map outputs=16
                GC time elapsed (ms)=826
                CPU time spent (ms)=13940
                Physical memory (bytes) snapshot=7531425792
                Virtual memory (bytes) snapshot=26764038144
                Total committed heap usage (bytes)=8563720192
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=1888
        File Output Format Counters
                Bytes Written=97
Job Finished in 26.69 seconds
Estimated value of Pi is 3.14250000000000000000
