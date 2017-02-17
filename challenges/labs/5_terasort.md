Terrasort
```
Last login: Fri Feb 17 06:15:38 2017 from 167.220.255.140
[raffles@ip-172-31-7-27 ~]$ kinit raffles@YABAR.SG
Password for raffles@YABAR.SG:
[raffles@ip-172-31-7-27 ~]$ klist
Ticket cache: FILE:/tmp/krb5cc_2000
Default principal: raffles@YABAR.SG

Valid starting     Expires            Service principal
02/17/17 07:08:18  02/18/17 07:08:18  krbtgt/YABAR.SG@YABAR.SG
        renew until 02/24/17 07:08:18
[raffles@ip-172-31-7-27 ~]$ hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /user/raffles/tgen512m /user/raffles/terasort_output
17/02/17 07:12:28 INFO terasort.TeraSort: starting
17/02/17 07:12:30 INFO input.FileInputFormat: Total input paths to process : 6
Spent 224ms computing base-splits.
Spent 4ms computing TeraScheduler splits.
Computing input splits took 229ms
Sampling 10 splits of 156
Making 8 from 100000 sampled records
Computing parititions took 851ms
Spent 1081ms computing partitions.
17/02/17 07:12:31 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-1-16.ap-southeast-1.compute.internal/172.31.1.16:8032
17/02/17 07:12:31 INFO mapreduce.JobSubmitter: number of splits:156
17/02/17 07:12:32 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1487311167324_0004
17/02/17 07:12:32 INFO impl.YarnClientImpl: Submitted application application_1487311167324_0004
17/02/17 07:12:32 INFO mapreduce.Job: The url to track the job: http://ip-172-31-1-16.ap-southeast-1.compute.internal:8088/proxy/application_1487311167324_0004/
17/02/17 07:12:32 INFO mapreduce.Job: Running job: job_1487311167324_0004
17/02/17 07:12:39 INFO mapreduce.Job: Job job_1487311167324_0004 running in uber mode : false
17/02/17 07:12:39 INFO mapreduce.Job:  map 0% reduce 0%
17/02/17 07:12:50 INFO mapreduce.Job:  map 1% reduce 0%
17/02/17 07:12:51 INFO mapreduce.Job:  map 5% reduce 0%
17/02/17 07:12:52 INFO mapreduce.Job:  map 6% reduce 0%
17/02/17 07:12:53 INFO mapreduce.Job:  map 8% reduce 0%
17/02/17 07:13:00 INFO mapreduce.Job:  map 10% reduce 0%
17/02/17 07:13:01 INFO mapreduce.Job:  map 12% reduce 0%
17/02/17 07:13:02 INFO mapreduce.Job:  map 13% reduce 0%
17/02/17 07:13:03 INFO mapreduce.Job:  map 14% reduce 0%
17/02/17 07:13:05 INFO mapreduce.Job:  map 15% reduce 0%
17/02/17 07:13:07 INFO mapreduce.Job:  map 17% reduce 0%
17/02/17 07:13:11 INFO mapreduce.Job:  map 19% reduce 0%
17/02/17 07:13:12 INFO mapreduce.Job:  map 20% reduce 0%
17/02/17 07:13:13 INFO mapreduce.Job:  map 21% reduce 0%
17/02/17 07:13:14 INFO mapreduce.Job:  map 22% reduce 0%
17/02/17 07:13:18 INFO mapreduce.Job:  map 23% reduce 0%
17/02/17 07:13:19 INFO mapreduce.Job:  map 24% reduce 0%
17/02/17 07:13:20 INFO mapreduce.Job:  map 26% reduce 0%
17/02/17 07:13:21 INFO mapreduce.Job:  map 27% reduce 0%
17/02/17 07:13:23 INFO mapreduce.Job:  map 28% reduce 0%
17/02/17 07:13:24 INFO mapreduce.Job:  map 30% reduce 0%
17/02/17 07:13:25 INFO mapreduce.Job:  map 31% reduce 0%
17/02/17 07:13:29 INFO mapreduce.Job:  map 32% reduce 0%
17/02/17 07:13:31 INFO mapreduce.Job:  map 33% reduce 0%
17/02/17 07:13:32 INFO mapreduce.Job:  map 35% reduce 0%
17/02/17 07:13:34 INFO mapreduce.Job:  map 37% reduce 0%
17/02/17 07:13:35 INFO mapreduce.Job:  map 38% reduce 0%
17/02/17 07:13:36 INFO mapreduce.Job:  map 39% reduce 0%
17/02/17 07:13:40 INFO mapreduce.Job:  map 40% reduce 0%
17/02/17 07:13:42 INFO mapreduce.Job:  map 41% reduce 0%
17/02/17 07:13:44 INFO mapreduce.Job:  map 42% reduce 0%
17/02/17 07:13:46 INFO mapreduce.Job:  map 46% reduce 0%
17/02/17 07:13:48 INFO mapreduce.Job:  map 47% reduce 0%
17/02/17 07:13:50 INFO mapreduce.Job:  map 49% reduce 0%
17/02/17 07:13:57 INFO mapreduce.Job:  map 52% reduce 0%
17/02/17 07:13:58 INFO mapreduce.Job:  map 53% reduce 0%
17/02/17 07:13:59 INFO mapreduce.Job:  map 56% reduce 0%
17/02/17 07:14:00 INFO mapreduce.Job:  map 57% reduce 0%
17/02/17 07:14:02 INFO mapreduce.Job:  map 58% reduce 0%
17/02/17 07:14:08 INFO mapreduce.Job:  map 60% reduce 0%
17/02/17 07:14:10 INFO mapreduce.Job:  map 63% reduce 0%
17/02/17 07:14:11 INFO mapreduce.Job:  map 64% reduce 0%
17/02/17 07:14:12 INFO mapreduce.Job:  map 66% reduce 0%
17/02/17 07:14:19 INFO mapreduce.Job:  map 68% reduce 0%
17/02/17 07:14:20 INFO mapreduce.Job:  map 69% reduce 0%
17/02/17 07:14:21 INFO mapreduce.Job:  map 72% reduce 0%
17/02/17 07:14:24 INFO mapreduce.Job:  map 73% reduce 0%
17/02/17 07:14:25 INFO mapreduce.Job:  map 74% reduce 0%
17/02/17 07:14:28 INFO mapreduce.Job:  map 75% reduce 0%
17/02/17 07:14:30 INFO mapreduce.Job:  map 78% reduce 0%
17/02/17 07:14:32 INFO mapreduce.Job:  map 79% reduce 0%
17/02/17 07:14:33 INFO mapreduce.Job:  map 81% reduce 0%
17/02/17 07:14:37 INFO mapreduce.Job:  map 82% reduce 0%
17/02/17 07:14:38 INFO mapreduce.Job:  map 83% reduce 0%
17/02/17 07:14:40 INFO mapreduce.Job:  map 85% reduce 0%
17/02/17 07:14:41 INFO mapreduce.Job:  map 87% reduce 0%
17/02/17 07:14:43 INFO mapreduce.Job:  map 88% reduce 0%
17/02/17 07:14:46 INFO mapreduce.Job:  map 89% reduce 0%
17/02/17 07:14:49 INFO mapreduce.Job:  map 90% reduce 0%
17/02/17 07:14:54 INFO mapreduce.Job:  map 91% reduce 0%
17/02/17 07:14:55 INFO mapreduce.Job:  map 92% reduce 0%
17/02/17 07:14:58 INFO mapreduce.Job:  map 94% reduce 12%
17/02/17 07:14:59 INFO mapreduce.Job:  map 94% reduce 19%
17/02/17 07:15:01 INFO mapreduce.Job:  map 94% reduce 27%
17/02/17 07:15:04 INFO mapreduce.Job:  map 96% reduce 27%
17/02/17 07:15:05 INFO mapreduce.Job:  map 98% reduce 28%
17/02/17 07:15:11 INFO mapreduce.Job:  map 99% reduce 29%
17/02/17 07:15:12 INFO mapreduce.Job:  map 100% reduce 29%
17/02/17 07:15:16 INFO mapreduce.Job:  map 100% reduce 41%
17/02/17 07:15:17 INFO mapreduce.Job:  map 100% reduce 50%
17/02/17 07:15:19 INFO mapreduce.Job:  map 100% reduce 58%
17/02/17 07:15:22 INFO mapreduce.Job:  map 100% reduce 63%
17/02/17 07:15:23 INFO mapreduce.Job:  map 100% reduce 75%
17/02/17 07:15:25 INFO mapreduce.Job:  map 100% reduce 80%
17/02/17 07:15:28 INFO mapreduce.Job:  map 100% reduce 89%
17/02/17 07:15:29 INFO mapreduce.Job:  map 100% reduce 92%
17/02/17 07:15:30 INFO mapreduce.Job:  map 100% reduce 93%
17/02/17 07:15:31 INFO mapreduce.Job:  map 100% reduce 97%
17/02/17 07:15:35 INFO mapreduce.Job:  map 100% reduce 99%
17/02/17 07:15:36 INFO mapreduce.Job:  map 100% reduce 100%
17/02/17 07:15:36 INFO mapreduce.Job: Job job_1487311167324_0004 completed successfully
17/02/17 07:15:36 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=2285771932
                FILE: Number of bytes written=4546595840
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=5120024648
                HDFS: Number of bytes written=5120000000
                HDFS: Number of read operations=492
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=156
                Launched reduce tasks=8
                Data-local map tasks=154
                Rack-local map tasks=2
                Total time spent by all maps in occupied slots (ms)=1552650
                Total time spent by all reduces in occupied slots (ms)=380158
                Total time spent by all map tasks (ms)=1552650
                Total time spent by all reduce tasks (ms)=380158
                Total vcore-seconds taken by all map tasks=1552650
                Total vcore-seconds taken by all reduce tasks=380158
                Total megabyte-seconds taken by all map tasks=1589913600
                Total megabyte-seconds taken by all reduce tasks=389281792
        Map-Reduce Framework
                Map input records=51200000
                Map output records=51200000
                Map output bytes=5222400000
                Map output materialized bytes=2240103638
                Input split bytes=24648
                Combine input records=0
                Combine output records=0
                Reduce input groups=51200000
                Reduce shuffle bytes=2240103638
                Reduce input records=51200000
                Reduce output records=51200000
                Spilled Records=102400000
                Shuffled Maps =1248
                Failed Shuffles=0
                Merged Map outputs=1248
                GC time elapsed (ms)=24414
                CPU time spent (ms)=817560
                Physical memory (bytes) snapshot=82813661184
                Virtual memory (bytes) snapshot=257612427264
                Total committed heap usage (bytes)=94261739520
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=5120000000
        File Output Format Counters
                Bytes Written=5120000000
17/02/17 07:15:36 INFO terasort.TeraSort: done
```