```
[raffles@ip-172-31-7-27 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -D mapreduce.job.maps=6 -D dfs.block.size=33554432 51200000 /user/raffles/tgen512m
17/02/17 06:26:30 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8032
17/02/17 06:26:31 INFO terasort.TeraGen: Generating 51200000 using 6
17/02/17 06:26:31 INFO mapreduce.JobSubmitter: number of splits:6
17/02/17 06:26:31 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/02/17 06:26:31 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1487311167324_0003
17/02/17 06:26:32 INFO impl.YarnClientImpl: Submitted application application_1487311167324_0003
17/02/17 06:26:32 INFO mapreduce.Job: The url to track the job: http://ip-172-31-1-16.ap-southeast-1.compute.internal:8088/proxy/application_1487311167324_0003/
17/02/17 06:26:32 INFO mapreduce.Job: Running job: job_1487311167324_0003
17/02/17 06:26:39 INFO mapreduce.Job: Job job_1487311167324_0003 running in uber mode : false
17/02/17 06:26:39 INFO mapreduce.Job:  map 0% reduce 0%
17/02/17 06:26:57 INFO mapreduce.Job:  map 26% reduce 0%
17/02/17 06:26:58 INFO mapreduce.Job:  map 37% reduce 0%
17/02/17 06:27:03 INFO mapreduce.Job:  map 44% reduce 0%
17/02/17 06:27:04 INFO mapreduce.Job:  map 48% reduce 0%
17/02/17 06:27:09 INFO mapreduce.Job:  map 56% reduce 0%
17/02/17 06:27:10 INFO mapreduce.Job:  map 57% reduce 0%
17/02/17 06:27:15 INFO mapreduce.Job:  map 67% reduce 0%
17/02/17 06:27:21 INFO mapreduce.Job:  map 81% reduce 0%
17/02/17 06:27:28 INFO mapreduce.Job:  map 91% reduce 0%
17/02/17 06:27:32 INFO mapreduce.Job:  map 93% reduce 0%
17/02/17 06:27:33 INFO mapreduce.Job:  map 95% reduce 0%
17/02/17 06:27:34 INFO mapreduce.Job:  map 99% reduce 0%
17/02/17 06:27:35 INFO mapreduce.Job:  map 100% reduce 0%
17/02/17 06:27:35 INFO mapreduce.Job: Job job_1487311167324_0003 completed successfully
17/02/17 06:27:35 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=748896
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=511
                HDFS: Number of bytes written=5120000000
                HDFS: Number of read operations=24
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=12
        Job Counters
                Launched map tasks=6
                Other local map tasks=6
                Total time spent by all maps in occupied slots (ms)=311822
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=311822
                Total vcore-seconds taken by all map tasks=311822
                Total megabyte-seconds taken by all map tasks=319305728
        Map-Reduce Framework
                Map input records=51200000
                Map output records=51200000
                Input split bytes=511
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1138
                CPU time spent (ms)=101120
                Physical memory (bytes) snapshot=2090328064
                Virtual memory (bytes) snapshot=9411739648
                Total committed heap usage (bytes)=2168455168
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=109963291816450258
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=5120000000

real    1m7.389s
user    0m6.007s
sys     0m0.658s
[raffles@ip-172-31-7-27 ~]$ hdfs dfs -ls /user/raffles/tgen512m/
Found 7 items
-rw-r--r--   3 raffles raffles          0 2017-02-17 06:27 /user/raffles/tgen512m/_SUCCESS
-rw-r--r--   3 raffles raffles  853333400 2017-02-17 06:27 /user/raffles/tgen512m/part-m-00000
-rw-r--r--   3 raffles raffles  853333300 2017-02-17 06:27 /user/raffles/tgen512m/part-m-00001
-rw-r--r--   3 raffles raffles  853333300 2017-02-17 06:27 /user/raffles/tgen512m/part-m-00002
-rw-r--r--   3 raffles raffles  853333400 2017-02-17 06:27 /user/raffles/tgen512m/part-m-00003
-rw-r--r--   3 raffles raffles  853333300 2017-02-17 06:27 /user/raffles/tgen512m/part-m-00004
-rw-r--r--   3 raffles raffles  853333300 2017-02-17 06:27 /user/raffles/tgen512m/part-m-00005
```