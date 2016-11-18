```
[bavaria@ip-172-31-56-113 ~]$ hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /user/bavaria/tgen512m /user/bavaria/tsort512m
16/11/18 15:36:46 INFO terasort.TeraSort: starting
16/11/18 15:36:48 INFO hdfs.DFSClient: Created token for bavaria: HDFS_DELEGATION_TOKEN owner=bavaria@AG35.IL, renewer=yarn, realUser=, issueDate=1479501408314, maxDate=1480106208314, sequenceNumber=1, masterKeyId=2 on 172.31.56.113:8020
16/11/18 15:36:48 INFO security.TokenCache: Got dt for hdfs://ip-172-31-56-113.ec2.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.56.113:8020, Ident: (token for bavaria: HDFS_DELEGATION_TOKEN owner=bavaria@AG35.IL, renewer=yarn, realUser=, issueDate=1479501408314, maxDate=1480106208314, sequenceNumber=1, masterKeyId=2)
16/11/18 15:36:48 INFO input.FileInputFormat: Total input paths to process : 2
Spent 468ms computing base-splits.
Spent 5ms computing TeraScheduler splits.
Computing input splits took 473ms
Sampling 10 splits of 306
Making 10 from 100000 sampled records
Computing parititions took 1311ms
Spent 1788ms computing partitions.
16/11/18 15:36:50 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-56-113.ec2.internal/172.31.56.113:8032
16/11/18 15:36:50 INFO mapreduce.JobSubmitter: number of splits:306
16/11/18 15:36:50 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1479500950411_0001
16/11/18 15:36:50 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.56.113:8020, Ident: (token for bavaria: HDFS_DELEGATION_TOKEN owner=bavaria@AG35.IL, renewer=yarn, realUser=, issueDate=1479501408314, maxDate=1480106208314, sequenceNumber=1, masterKeyId=2)
16/11/18 15:36:51 INFO impl.YarnClientImpl: Submitted application application_1479500950411_0001
16/11/18 15:36:51 INFO mapreduce.Job: The url to track the job: http://ip-172-31-56-113.ec2.internal:8088/proxy/application_1479500950411_0001/
16/11/18 15:36:51 INFO mapreduce.Job: Running job: job_1479500950411_0001
16/11/18 15:37:02 INFO mapreduce.Job: Job job_1479500950411_0001 running in uber mode : false
16/11/18 15:37:02 INFO mapreduce.Job:  map 0% reduce 0%
16/11/18 15:37:11 INFO mapreduce.Job:  map 1% reduce 0%
16/11/18 15:37:16 INFO mapreduce.Job:  map 3% reduce 0%
16/11/18 15:37:20 INFO mapreduce.Job:  map 4% reduce 0%
16/11/18 15:37:25 INFO mapreduce.Job:  map 6% reduce 0%
16/11/18 15:37:28 INFO mapreduce.Job:  map 7% reduce 0%
16/11/18 15:37:33 INFO mapreduce.Job:  map 8% reduce 0%
16/11/18 15:37:34 INFO mapreduce.Job:  map 9% reduce 0%
16/11/18 15:37:39 INFO mapreduce.Job:  map 10% reduce 0%
16/11/18 15:37:43 INFO mapreduce.Job:  map 12% reduce 0%
16/11/18 15:37:49 INFO mapreduce.Job:  map 13% reduce 0%
16/11/18 15:37:50 INFO mapreduce.Job:  map 14% reduce 0%
16/11/18 15:37:52 INFO mapreduce.Job:  map 15% reduce 0%
16/11/18 15:37:57 INFO mapreduce.Job:  map 16% reduce 0%
16/11/18 15:37:59 INFO mapreduce.Job:  map 17% reduce 0%
16/11/18 15:38:01 INFO mapreduce.Job:  map 18% reduce 0%
16/11/18 15:38:05 INFO mapreduce.Job:  map 19% reduce 0%
16/11/18 15:38:07 INFO mapreduce.Job:  map 20% reduce 0%
16/11/18 15:38:09 INFO mapreduce.Job:  map 21% reduce 0%
16/11/18 15:38:13 INFO mapreduce.Job:  map 22% reduce 0%
16/11/18 15:38:15 INFO mapreduce.Job:  map 23% reduce 0%
16/11/18 15:38:18 INFO mapreduce.Job:  map 24% reduce 0%
16/11/18 15:38:21 INFO mapreduce.Job:  map 25% reduce 0%
16/11/18 15:38:25 INFO mapreduce.Job:  map 26% reduce 0%
16/11/18 15:38:29 INFO mapreduce.Job:  map 27% reduce 0%
16/11/18 15:38:31 INFO mapreduce.Job:  map 28% reduce 0%
16/11/18 15:38:36 INFO mapreduce.Job:  map 29% reduce 0%
16/11/18 15:38:37 INFO mapreduce.Job:  map 30% reduce 0%
16/11/18 15:38:39 INFO mapreduce.Job:  map 31% reduce 0%
16/11/18 15:38:43 INFO mapreduce.Job:  map 32% reduce 0%
16/11/18 15:38:46 INFO mapreduce.Job:  map 33% reduce 0%
16/11/18 15:38:49 INFO mapreduce.Job:  map 34% reduce 0%
16/11/18 15:38:51 INFO mapreduce.Job:  map 35% reduce 0%
16/11/18 15:38:55 INFO mapreduce.Job:  map 36% reduce 0%
16/11/18 15:38:57 INFO mapreduce.Job:  map 37% reduce 0%
16/11/18 15:39:02 INFO mapreduce.Job:  map 38% reduce 0%
16/11/18 15:39:04 INFO mapreduce.Job:  map 39% reduce 0%
16/11/18 15:39:06 INFO mapreduce.Job:  map 40% reduce 0%
16/11/18 15:39:12 INFO mapreduce.Job:  map 41% reduce 0%
16/11/18 15:39:13 INFO mapreduce.Job:  map 42% reduce 0%
16/11/18 15:39:19 INFO mapreduce.Job:  map 43% reduce 0%
16/11/18 15:39:23 INFO mapreduce.Job:  map 44% reduce 0%
16/11/18 15:39:26 INFO mapreduce.Job:  map 45% reduce 0%
16/11/18 15:39:31 INFO mapreduce.Job:  map 46% reduce 0%
16/11/18 15:39:33 INFO mapreduce.Job:  map 47% reduce 0%
16/11/18 15:39:37 INFO mapreduce.Job:  map 48% reduce 0%
16/11/18 15:39:39 INFO mapreduce.Job:  map 49% reduce 0%
16/11/18 15:39:41 INFO mapreduce.Job:  map 50% reduce 0%
16/11/18 15:39:44 INFO mapreduce.Job:  map 51% reduce 0%
16/11/18 15:39:47 INFO mapreduce.Job:  map 52% reduce 0%
16/11/18 15:39:49 INFO mapreduce.Job:  map 53% reduce 0%
16/11/18 15:39:53 INFO mapreduce.Job:  map 54% reduce 0%
16/11/18 15:39:55 INFO mapreduce.Job:  map 55% reduce 0%
16/11/18 15:39:59 INFO mapreduce.Job:  map 56% reduce 0%
16/11/18 15:40:01 INFO mapreduce.Job:  map 57% reduce 0%
16/11/18 15:40:05 INFO mapreduce.Job:  map 58% reduce 0%
16/11/18 15:40:07 INFO mapreduce.Job:  map 59% reduce 0%
16/11/18 15:40:11 INFO mapreduce.Job:  map 60% reduce 0%
16/11/18 15:40:14 INFO mapreduce.Job:  map 61% reduce 0%
16/11/18 15:40:15 INFO mapreduce.Job:  map 62% reduce 0%
16/11/18 15:40:19 INFO mapreduce.Job:  map 63% reduce 0%
16/11/18 15:40:22 INFO mapreduce.Job:  map 64% reduce 0%
16/11/18 15:40:25 INFO mapreduce.Job:  map 65% reduce 0%
16/11/18 15:40:27 INFO mapreduce.Job:  map 66% reduce 0%
16/11/18 15:40:31 INFO mapreduce.Job:  map 67% reduce 0%
16/11/18 15:40:32 INFO mapreduce.Job:  map 68% reduce 0%
16/11/18 15:40:37 INFO mapreduce.Job:  map 69% reduce 0%
16/11/18 15:40:38 INFO mapreduce.Job:  map 70% reduce 0%
16/11/18 15:40:42 INFO mapreduce.Job:  map 71% reduce 0%
16/11/18 15:40:45 INFO mapreduce.Job:  map 72% reduce 0%
16/11/18 15:40:48 INFO mapreduce.Job:  map 73% reduce 0%
16/11/18 15:40:50 INFO mapreduce.Job:  map 74% reduce 0%
16/11/18 15:40:53 INFO mapreduce.Job:  map 75% reduce 0%
16/11/18 15:40:56 INFO mapreduce.Job:  map 76% reduce 0%
16/11/18 15:40:59 INFO mapreduce.Job:  map 77% reduce 0%
16/11/18 15:41:02 INFO mapreduce.Job:  map 78% reduce 0%
16/11/18 15:41:04 INFO mapreduce.Job:  map 79% reduce 0%
16/11/18 15:41:08 INFO mapreduce.Job:  map 80% reduce 0%
16/11/18 15:41:10 INFO mapreduce.Job:  map 81% reduce 0%
16/11/18 15:41:14 INFO mapreduce.Job:  map 82% reduce 0%
16/11/18 15:41:16 INFO mapreduce.Job:  map 83% reduce 0%
16/11/18 15:41:21 INFO mapreduce.Job:  map 84% reduce 0%
16/11/18 15:41:22 INFO mapreduce.Job:  map 84% reduce 3%
16/11/18 15:41:24 INFO mapreduce.Job:  map 84% reduce 6%
16/11/18 15:41:27 INFO mapreduce.Job:  map 84% reduce 8%
16/11/18 15:41:28 INFO mapreduce.Job:  map 85% reduce 14%
16/11/18 15:41:34 INFO mapreduce.Job:  map 86% reduce 14%
16/11/18 15:41:40 INFO mapreduce.Job:  map 87% reduce 14%
16/11/18 15:41:46 INFO mapreduce.Job:  map 87% reduce 15%
16/11/18 15:41:47 INFO mapreduce.Job:  map 88% reduce 15%
16/11/18 15:41:55 INFO mapreduce.Job:  map 89% reduce 15%
16/11/18 15:42:02 INFO mapreduce.Job:  map 90% reduce 15%
16/11/18 15:42:08 INFO mapreduce.Job:  map 91% reduce 15%
16/11/18 15:42:15 INFO mapreduce.Job:  map 92% reduce 15%
16/11/18 15:42:25 INFO mapreduce.Job:  map 93% reduce 15%
16/11/18 15:42:30 INFO mapreduce.Job:  map 93% reduce 16%
16/11/18 15:42:32 INFO mapreduce.Job:  map 94% reduce 16%
16/11/18 15:42:40 INFO mapreduce.Job:  map 95% reduce 16%
16/11/18 15:42:47 INFO mapreduce.Job:  map 96% reduce 16%
16/11/18 15:42:54 INFO mapreduce.Job:  map 97% reduce 16%
16/11/18 15:43:01 INFO mapreduce.Job:  map 98% reduce 16%
16/11/18 15:43:07 INFO mapreduce.Job:  map 99% reduce 16%
16/11/18 15:43:11 INFO mapreduce.Job:  map 99% reduce 17%
16/11/18 15:43:15 INFO mapreduce.Job:  map 100% reduce 17%
16/11/18 15:43:16 INFO mapreduce.Job:  map 100% reduce 18%
16/11/18 15:43:17 INFO mapreduce.Job:  map 100% reduce 26%
16/11/18 15:43:19 INFO mapreduce.Job:  map 100% reduce 28%
16/11/18 15:43:20 INFO mapreduce.Job:  map 100% reduce 36%
16/11/18 15:43:22 INFO mapreduce.Job:  map 100% reduce 39%
16/11/18 15:43:23 INFO mapreduce.Job:  map 100% reduce 45%
16/11/18 15:43:25 INFO mapreduce.Job:  map 100% reduce 49%
16/11/18 15:43:26 INFO mapreduce.Job:  map 100% reduce 59%
16/11/18 15:43:27 INFO mapreduce.Job:  map 100% reduce 60%
16/11/18 15:43:28 INFO mapreduce.Job:  map 100% reduce 66%
16/11/18 15:43:29 INFO mapreduce.Job:  map 100% reduce 68%
16/11/18 15:43:31 INFO mapreduce.Job:  map 100% reduce 73%
16/11/18 15:43:32 INFO mapreduce.Job:  map 100% reduce 75%
16/11/18 15:43:33 INFO mapreduce.Job:  map 100% reduce 76%
16/11/18 15:43:34 INFO mapreduce.Job:  map 100% reduce 78%
16/11/18 15:43:35 INFO mapreduce.Job:  map 100% reduce 83%
16/11/18 15:43:37 INFO mapreduce.Job:  map 100% reduce 85%
16/11/18 15:43:38 INFO mapreduce.Job:  map 100% reduce 91%
16/11/18 15:43:41 INFO mapreduce.Job:  map 100% reduce 95%
16/11/18 15:43:44 INFO mapreduce.Job:  map 100% reduce 98%
16/11/18 15:43:50 INFO mapreduce.Job:  map 100% reduce 99%
16/11/18 15:43:52 INFO mapreduce.Job:  map 100% reduce 100%
16/11/18 15:43:55 INFO mapreduce.Job: Job job_1479500950411_0001 completed successfully
16/11/18 15:43:55 INFO mapreduce.Job: Counters: 50
        File System Counters
                FILE: Number of bytes read=2285367674
                FILE: Number of bytes written=4561634664
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=5120043146
                HDFS: Number of bytes written=5120000000
                HDFS: Number of read operations=948
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=20
        Job Counters
                Launched map tasks=306
                Launched reduce tasks=10
                Data-local map tasks=303
                Rack-local map tasks=3
                Total time spent by all maps in occupied slots (ms)=1834579
                Total time spent by all reduces in occupied slots (ms)=755931
                Total time spent by all map tasks (ms)=1834579
                Total time spent by all reduce tasks (ms)=755931
                Total vcore-seconds taken by all map tasks=1834579
                Total vcore-seconds taken by all reduce tasks=755931
                Total megabyte-seconds taken by all map tasks=1878608896
                Total megabyte-seconds taken by all reduce tasks=774073344
        Map-Reduce Framework
                Map input records=51200000
                Map output records=51200000
                Map output bytes=5222400000
                Map output materialized bytes=2237814484
                Input split bytes=43146
                Combine input records=0
                Combine output records=0
                Reduce input groups=51200000
                Reduce shuffle bytes=2237814484
                Reduce input records=51200000
                Reduce output records=51200000
                Spilled Records=102400000
                Shuffled Maps =3060
                Failed Shuffles=0
                Merged Map outputs=3060
                GC time elapsed (ms)=21976
                CPU time spent (ms)=1095650
                Physical memory (bytes) snapshot=150320566272
                Virtual memory (bytes) snapshot=495497555968
                Total committed heap usage (bytes)=179299155968
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
16/11/18 15:43:55 INFO terasort.TeraSort: done
```