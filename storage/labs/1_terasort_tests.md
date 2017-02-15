teragen time
```
real    1m56.598s
user    0m6.038s
sys     0m0.749s
```

terasort time
```
real    5m41.858s
user    0m10.083s
sys     0m0.917s
```


Console output
```
[yabar@ip-172-31-14-10 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Dmapreduce.job.maps=4 -Ddfs.blocksize=33554432 100000000 /tmp/yabar/teragen_output
17/02/15 06:33:20 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-14-10.ap-southeast-1.compute.internal/172.31.14.10:8032
17/02/15 06:33:21 INFO terasort.TeraSort: Generating 100000000 using 4
17/02/15 06:33:21 INFO mapreduce.JobSubmitter: number of splits:4
17/02/15 06:33:21 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1487129473337_0003
17/02/15 06:33:21 INFO impl.YarnClientImpl: Submitted application application_1487129473337_0003
17/02/15 06:33:21 INFO mapreduce.Job: The url to track the job: http://ip-172-31-14-10.ap-southeast-1.compute.internal:8088/proxy/application_1487129473337_0003/
17/02/15 06:33:21 INFO mapreduce.Job: Running job: job_1487129473337_0003
17/02/15 06:33:28 INFO mapreduce.Job: Job job_1487129473337_0003 running in uber mode : false
17/02/15 06:33:28 INFO mapreduce.Job:  map 0% reduce 0%
17/02/15 06:33:40 INFO mapreduce.Job:  map 10% reduce 0%
17/02/15 06:33:41 INFO mapreduce.Job:  map 13% reduce 0%
17/02/15 06:33:43 INFO mapreduce.Job:  map 18% reduce 0%
17/02/15 06:33:44 INFO mapreduce.Job:  map 19% reduce 0%
17/02/15 06:33:46 INFO mapreduce.Job:  map 21% reduce 0%
17/02/15 06:33:47 INFO mapreduce.Job:  map 22% reduce 0%
17/02/15 06:33:49 INFO mapreduce.Job:  map 24% reduce 0%
17/02/15 06:33:52 INFO mapreduce.Job:  map 26% reduce 0%
17/02/15 06:33:53 INFO mapreduce.Job:  map 27% reduce 0%
17/02/15 06:33:55 INFO mapreduce.Job:  map 29% reduce 0%
17/02/15 06:33:56 INFO mapreduce.Job:  map 30% reduce 0%
17/02/15 06:33:58 INFO mapreduce.Job:  map 31% reduce 0%
17/02/15 06:33:59 INFO mapreduce.Job:  map 32% reduce 0%
17/02/15 06:34:01 INFO mapreduce.Job:  map 34% reduce 0%
17/02/15 06:34:02 INFO mapreduce.Job:  map 35% reduce 0%
17/02/15 06:34:04 INFO mapreduce.Job:  map 38% reduce 0%
17/02/15 06:34:05 INFO mapreduce.Job:  map 39% reduce 0%
17/02/15 06:34:07 INFO mapreduce.Job:  map 40% reduce 0%
17/02/15 06:34:08 INFO mapreduce.Job:  map 41% reduce 0%
17/02/15 06:34:10 INFO mapreduce.Job:  map 43% reduce 0%
17/02/15 06:34:11 INFO mapreduce.Job:  map 44% reduce 0%
17/02/15 06:34:13 INFO mapreduce.Job:  map 46% reduce 0%
17/02/15 06:34:14 INFO mapreduce.Job:  map 47% reduce 0%
17/02/15 06:34:16 INFO mapreduce.Job:  map 48% reduce 0%
17/02/15 06:34:17 INFO mapreduce.Job:  map 49% reduce 0%
17/02/15 06:34:19 INFO mapreduce.Job:  map 51% reduce 0%
17/02/15 06:34:20 INFO mapreduce.Job:  map 52% reduce 0%
17/02/15 06:34:22 INFO mapreduce.Job:  map 54% reduce 0%
17/02/15 06:34:23 INFO mapreduce.Job:  map 55% reduce 0%
17/02/15 06:34:25 INFO mapreduce.Job:  map 57% reduce 0%
17/02/15 06:34:26 INFO mapreduce.Job:  map 58% reduce 0%
17/02/15 06:34:28 INFO mapreduce.Job:  map 60% reduce 0%
17/02/15 06:34:29 INFO mapreduce.Job:  map 61% reduce 0%
17/02/15 06:34:31 INFO mapreduce.Job:  map 62% reduce 0%
17/02/15 06:34:32 INFO mapreduce.Job:  map 63% reduce 0%
17/02/15 06:34:34 INFO mapreduce.Job:  map 65% reduce 0%
17/02/15 06:34:37 INFO mapreduce.Job:  map 67% reduce 0%
17/02/15 06:34:38 INFO mapreduce.Job:  map 68% reduce 0%
17/02/15 06:34:40 INFO mapreduce.Job:  map 70% reduce 0%
17/02/15 06:34:41 INFO mapreduce.Job:  map 71% reduce 0%
17/02/15 06:34:43 INFO mapreduce.Job:  map 74% reduce 0%
17/02/15 06:34:44 INFO mapreduce.Job:  map 75% reduce 0%
17/02/15 06:34:46 INFO mapreduce.Job:  map 77% reduce 0%
17/02/15 06:34:49 INFO mapreduce.Job:  map 80% reduce 0%
17/02/15 06:34:50 INFO mapreduce.Job:  map 81% reduce 0%
17/02/15 06:34:52 INFO mapreduce.Job:  map 83% reduce 0%
17/02/15 06:34:55 INFO mapreduce.Job:  map 85% reduce 0%
17/02/15 06:34:56 INFO mapreduce.Job:  map 86% reduce 0%
17/02/15 06:34:58 INFO mapreduce.Job:  map 88% reduce 0%
17/02/15 06:34:59 INFO mapreduce.Job:  map 89% reduce 0%
17/02/15 06:35:02 INFO mapreduce.Job:  map 91% reduce 0%
17/02/15 06:35:03 INFO mapreduce.Job:  map 92% reduce 0%
17/02/15 06:35:05 INFO mapreduce.Job:  map 93% reduce 0%
17/02/15 06:35:06 INFO mapreduce.Job:  map 94% reduce 0%
17/02/15 06:35:08 INFO mapreduce.Job:  map 96% reduce 0%
17/02/15 06:35:09 INFO mapreduce.Job:  map 97% reduce 0%
17/02/15 06:35:11 INFO mapreduce.Job:  map 99% reduce 0%
17/02/15 06:35:13 INFO mapreduce.Job:  map 100% reduce 0%
17/02/15 06:35:14 INFO mapreduce.Job: Job job_1487129473337_0003 completed successfully
17/02/15 06:35:14 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=498840
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=344
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=16
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=8
        Job Counters
                Launched map tasks=4
                Other local map tasks=4
                Total time spent by all maps in occupied slots (ms)=402573
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=402573
                Total vcore-seconds taken by all map tasks=402573
                Total megabyte-seconds taken by all map tasks=412234752
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Input split bytes=344
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1698
                CPU time spent (ms)=155890
                Physical memory (bytes) snapshot=803635200
                Virtual memory (bytes) snapshot=6282567680
                Total committed heap usage (bytes)=922222592
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=214760662691937609
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=10000000000

real    1m56.598s
user    0m6.038s
sys     0m0.749s
[yabar@ip-172-31-14-10 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /tmp/yabar/teragen_output /tmp/yabar/terasort_output
17/02/15 06:38:56 INFO terasort.TeraSort: starting
17/02/15 06:38:58 INFO input.FileInputFormat: Total input paths to process : 4
Spent 350ms computing base-splits.
Spent 7ms computing TeraScheduler splits.
Computing input splits took 358ms
Sampling 10 splits of 300
Making 8 from 100000 sampled records
Computing parititions took 1174ms
Spent 1535ms computing partitions.
17/02/15 06:39:00 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-14-10.ap-southeast-1.compute.internal/172.31.14.10:8032
17/02/15 06:39:00 INFO mapreduce.JobSubmitter: number of splits:300
17/02/15 06:39:00 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1487129473337_0004
17/02/15 06:39:01 INFO impl.YarnClientImpl: Submitted application application_1487129473337_0004
17/02/15 06:39:01 INFO mapreduce.Job: The url to track the job: http://ip-172-31-14-10.ap-southeast-1.compute.internal:8088/proxy/application_1487129473337_0004/
17/02/15 06:39:01 INFO mapreduce.Job: Running job: job_1487129473337_0004
17/02/15 06:39:07 INFO mapreduce.Job: Job job_1487129473337_0004 running in uber mode : false
17/02/15 06:39:07 INFO mapreduce.Job:  map 0% reduce 0%
17/02/15 06:39:20 INFO mapreduce.Job:  map 1% reduce 0%
17/02/15 06:39:22 INFO mapreduce.Job:  map 5% reduce 0%
17/02/15 06:39:30 INFO mapreduce.Job:  map 6% reduce 0%
17/02/15 06:39:35 INFO mapreduce.Job:  map 9% reduce 0%
17/02/15 06:39:36 INFO mapreduce.Job:  map 10% reduce 0%
17/02/15 06:39:41 INFO mapreduce.Job:  map 11% reduce 0%
17/02/15 06:39:48 INFO mapreduce.Job:  map 12% reduce 0%
17/02/15 06:39:49 INFO mapreduce.Job:  map 15% reduce 0%
17/02/15 06:39:51 INFO mapreduce.Job:  map 16% reduce 0%
17/02/15 06:40:00 INFO mapreduce.Job:  map 17% reduce 0%
17/02/15 06:40:02 INFO mapreduce.Job:  map 21% reduce 0%
17/02/15 06:40:11 INFO mapreduce.Job:  map 22% reduce 0%
17/02/15 06:40:13 INFO mapreduce.Job:  map 23% reduce 0%
17/02/15 06:40:15 INFO mapreduce.Job:  map 24% reduce 0%
17/02/15 06:40:16 INFO mapreduce.Job:  map 26% reduce 0%
17/02/15 06:40:21 INFO mapreduce.Job:  map 27% reduce 0%
17/02/15 06:40:27 INFO mapreduce.Job:  map 28% reduce 0%
17/02/15 06:40:28 INFO mapreduce.Job:  map 29% reduce 0%
17/02/15 06:40:29 INFO mapreduce.Job:  map 31% reduce 0%
17/02/15 06:40:32 INFO mapreduce.Job:  map 32% reduce 0%
17/02/15 06:40:40 INFO mapreduce.Job:  map 33% reduce 0%
17/02/15 06:40:41 INFO mapreduce.Job:  map 34% reduce 0%
17/02/15 06:40:42 INFO mapreduce.Job:  map 36% reduce 0%
17/02/15 06:40:43 INFO mapreduce.Job:  map 37% reduce 0%
17/02/15 06:40:51 INFO mapreduce.Job:  map 38% reduce 0%
17/02/15 06:40:53 INFO mapreduce.Job:  map 39% reduce 0%
17/02/15 06:40:54 INFO mapreduce.Job:  map 40% reduce 0%
17/02/15 06:40:55 INFO mapreduce.Job:  map 42% reduce 0%
17/02/15 06:41:01 INFO mapreduce.Job:  map 43% reduce 0%
17/02/15 06:41:05 INFO mapreduce.Job:  map 44% reduce 0%
17/02/15 06:41:07 INFO mapreduce.Job:  map 45% reduce 0%
17/02/15 06:41:08 INFO mapreduce.Job:  map 47% reduce 0%
17/02/15 06:41:10 INFO mapreduce.Job:  map 48% reduce 0%
17/02/15 06:41:17 INFO mapreduce.Job:  map 49% reduce 0%
17/02/15 06:41:19 INFO mapreduce.Job:  map 50% reduce 0%
17/02/15 06:41:20 INFO mapreduce.Job:  map 51% reduce 0%
17/02/15 06:41:21 INFO mapreduce.Job:  map 52% reduce 0%
17/02/15 06:41:22 INFO mapreduce.Job:  map 53% reduce 0%
17/02/15 06:41:28 INFO mapreduce.Job:  map 54% reduce 0%
17/02/15 06:41:32 INFO mapreduce.Job:  map 55% reduce 0%
17/02/15 06:41:33 INFO mapreduce.Job:  map 56% reduce 0%
17/02/15 06:41:34 INFO mapreduce.Job:  map 57% reduce 0%
17/02/15 06:41:35 INFO mapreduce.Job:  map 58% reduce 0%
17/02/15 06:41:39 INFO mapreduce.Job:  map 59% reduce 0%
17/02/15 06:41:43 INFO mapreduce.Job:  map 60% reduce 0%
17/02/15 06:41:46 INFO mapreduce.Job:  map 61% reduce 0%
17/02/15 06:41:47 INFO mapreduce.Job:  map 63% reduce 0%
17/02/15 06:41:51 INFO mapreduce.Job:  map 64% reduce 0%
17/02/15 06:41:54 INFO mapreduce.Job:  map 65% reduce 0%
17/02/15 06:41:59 INFO mapreduce.Job:  map 66% reduce 0%
17/02/15 06:42:00 INFO mapreduce.Job:  map 67% reduce 0%
17/02/15 06:42:01 INFO mapreduce.Job:  map 69% reduce 0%
17/02/15 06:42:05 INFO mapreduce.Job:  map 70% reduce 0%
17/02/15 06:42:11 INFO mapreduce.Job:  map 71% reduce 0%
17/02/15 06:42:12 INFO mapreduce.Job:  map 72% reduce 0%
17/02/15 06:42:13 INFO mapreduce.Job:  map 73% reduce 0%
17/02/15 06:42:14 INFO mapreduce.Job:  map 74% reduce 0%
17/02/15 06:42:16 INFO mapreduce.Job:  map 75% reduce 0%
17/02/15 06:42:22 INFO mapreduce.Job:  map 76% reduce 0%
17/02/15 06:42:25 INFO mapreduce.Job:  map 77% reduce 0%
17/02/15 06:42:26 INFO mapreduce.Job:  map 78% reduce 0%
17/02/15 06:42:27 INFO mapreduce.Job:  map 80% reduce 0%
17/02/15 06:42:32 INFO mapreduce.Job:  map 81% reduce 0%
17/02/15 06:42:38 INFO mapreduce.Job:  map 82% reduce 0%
17/02/15 06:42:39 INFO mapreduce.Job:  map 83% reduce 0%
17/02/15 06:42:40 INFO mapreduce.Job:  map 84% reduce 0%
17/02/15 06:42:41 INFO mapreduce.Job:  map 85% reduce 0%
17/02/15 06:42:43 INFO mapreduce.Job:  map 85% reduce 2%
17/02/15 06:42:46 INFO mapreduce.Job:  map 85% reduce 4%
17/02/15 06:42:49 INFO mapreduce.Job:  map 85% reduce 6%
17/02/15 06:42:50 INFO mapreduce.Job:  map 85% reduce 9%
17/02/15 06:42:52 INFO mapreduce.Job:  map 85% reduce 12%
17/02/15 06:42:53 INFO mapreduce.Job:  map 85% reduce 14%
17/02/15 06:42:54 INFO mapreduce.Job:  map 86% reduce 16%
17/02/15 06:42:55 INFO mapreduce.Job:  map 88% reduce 17%
17/02/15 06:42:56 INFO mapreduce.Job:  map 88% reduce 18%
17/02/15 06:42:58 INFO mapreduce.Job:  map 88% reduce 19%
17/02/15 06:42:59 INFO mapreduce.Job:  map 88% reduce 21%
17/02/15 06:43:00 INFO mapreduce.Job:  map 88% reduce 22%
17/02/15 06:43:02 INFO mapreduce.Job:  map 88% reduce 23%
17/02/15 06:43:05 INFO mapreduce.Job:  map 88% reduce 25%
17/02/15 06:43:06 INFO mapreduce.Job:  map 88% reduce 26%
17/02/15 06:43:07 INFO mapreduce.Job:  map 89% reduce 26%
17/02/15 06:43:08 INFO mapreduce.Job:  map 90% reduce 26%
17/02/15 06:43:15 INFO mapreduce.Job:  map 91% reduce 26%
17/02/15 06:43:18 INFO mapreduce.Job:  map 92% reduce 27%
17/02/15 06:43:23 INFO mapreduce.Job:  map 93% reduce 27%
17/02/15 06:43:27 INFO mapreduce.Job:  map 94% reduce 27%
17/02/15 06:43:28 INFO mapreduce.Job:  map 95% reduce 27%
17/02/15 06:43:30 INFO mapreduce.Job:  map 95% reduce 28%
17/02/15 06:43:36 INFO mapreduce.Job:  map 96% reduce 28%
17/02/15 06:43:37 INFO mapreduce.Job:  map 97% reduce 28%
17/02/15 06:43:41 INFO mapreduce.Job:  map 98% reduce 28%
17/02/15 06:43:48 INFO mapreduce.Job:  map 100% reduce 29%
17/02/15 06:43:50 INFO mapreduce.Job:  map 100% reduce 32%
17/02/15 06:43:51 INFO mapreduce.Job:  map 100% reduce 42%
17/02/15 06:43:52 INFO mapreduce.Job:  map 100% reduce 49%
17/02/15 06:43:53 INFO mapreduce.Job:  map 100% reduce 55%
17/02/15 06:43:54 INFO mapreduce.Job:  map 100% reduce 60%
17/02/15 06:43:55 INFO mapreduce.Job:  map 100% reduce 62%
17/02/15 06:43:56 INFO mapreduce.Job:  map 100% reduce 63%
17/02/15 06:43:57 INFO mapreduce.Job:  map 100% reduce 65%
17/02/15 06:43:58 INFO mapreduce.Job:  map 100% reduce 66%
17/02/15 06:43:59 INFO mapreduce.Job:  map 100% reduce 67%
17/02/15 06:44:00 INFO mapreduce.Job:  map 100% reduce 68%
17/02/15 06:44:01 INFO mapreduce.Job:  map 100% reduce 69%
17/02/15 06:44:02 INFO mapreduce.Job:  map 100% reduce 70%
17/02/15 06:44:03 INFO mapreduce.Job:  map 100% reduce 72%
17/02/15 06:44:04 INFO mapreduce.Job:  map 100% reduce 73%
17/02/15 06:44:05 INFO mapreduce.Job:  map 100% reduce 74%
17/02/15 06:44:06 INFO mapreduce.Job:  map 100% reduce 75%
17/02/15 06:44:07 INFO mapreduce.Job:  map 100% reduce 80%
17/02/15 06:44:08 INFO mapreduce.Job:  map 100% reduce 81%
17/02/15 06:44:09 INFO mapreduce.Job:  map 100% reduce 82%
17/02/15 06:44:10 INFO mapreduce.Job:  map 100% reduce 83%
17/02/15 06:44:11 INFO mapreduce.Job:  map 100% reduce 84%
17/02/15 06:44:13 INFO mapreduce.Job:  map 100% reduce 86%
17/02/15 06:44:14 INFO mapreduce.Job:  map 100% reduce 87%
17/02/15 06:44:16 INFO mapreduce.Job:  map 100% reduce 88%
17/02/15 06:44:17 INFO mapreduce.Job:  map 100% reduce 89%
17/02/15 06:44:18 INFO mapreduce.Job:  map 100% reduce 90%
17/02/15 06:44:20 INFO mapreduce.Job:  map 100% reduce 92%
17/02/15 06:44:21 INFO mapreduce.Job:  map 100% reduce 93%
17/02/15 06:44:23 INFO mapreduce.Job:  map 100% reduce 95%
17/02/15 06:44:26 INFO mapreduce.Job:  map 100% reduce 96%
17/02/15 06:44:27 INFO mapreduce.Job:  map 100% reduce 97%
17/02/15 06:44:29 INFO mapreduce.Job:  map 100% reduce 98%
17/02/15 06:44:32 INFO mapreduce.Job:  map 100% reduce 99%
17/02/15 06:44:35 INFO mapreduce.Job:  map 100% reduce 100%
17/02/15 06:44:37 INFO mapreduce.Job: Job job_1487129473337_0004 completed successfully
17/02/15 06:44:37 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=4474735490
                FILE: Number of bytes written=8888825185
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=10000036600
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=924
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=300
                Launched reduce tasks=8
                Data-local map tasks=300
                Total time spent by all maps in occupied slots (ms)=3347146
                Total time spent by all reduces in occupied slots (ms)=803721
                Total time spent by all map tasks (ms)=3347146
                Total time spent by all reduce tasks (ms)=803721
                Total vcore-seconds taken by all map tasks=3347146
                Total vcore-seconds taken by all reduce tasks=803721
                Total megabyte-seconds taken by all map tasks=3427477504
                Total megabyte-seconds taken by all reduce tasks=823010304
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Map output bytes=10200000000
                Map output materialized bytes=4375223545
                Input split bytes=36600
                Combine input records=0
                Combine output records=0
                Reduce input groups=100000000
                Reduce shuffle bytes=4375223545
                Reduce input records=100000000
                Reduce output records=100000000
                Spilled Records=200000000
                Shuffled Maps =2400
                Failed Shuffles=0
                Merged Map outputs=2400
                GC time elapsed (ms)=45341
                CPU time spent (ms)=1587760
                Physical memory (bytes) snapshot=146065309696
                Virtual memory (bytes) snapshot=483630170112
                Total committed heap usage (bytes)=174760394752
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=10000000000
        File Output Format Counters
                Bytes Written=10000000000
17/02/15 06:44:37 INFO terasort.TeraSort: done
```
