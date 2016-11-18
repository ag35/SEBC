```
[bavaria@ip-172-31-56-113 ~]$ time hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -D dfs.block.size=16777216 51200000 /user/bavaria/tgen512m

16/11/18 15:13:35 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-56-113.ec2.internal/172.31.56.113:8032
16/11/18 15:13:36 INFO terasort.TeraSort: Generating 51200000 using 2
16/11/18 15:13:36 INFO mapreduce.JobSubmitter: number of splits:2
16/11/18 15:13:36 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
16/11/18 15:13:36 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1479497522730_0001
16/11/18 15:13:37 INFO impl.YarnClientImpl: Submitted application application_1479497522730_0001
16/11/18 15:13:37 INFO mapreduce.Job: The url to track the job: http://ip-172-31-56-113.ec2.internal:8088/proxy/application_1479497522730_0001/
16/11/18 15:13:37 INFO mapreduce.Job: Running job: job_1479497522730_0001
16/11/18 15:13:44 INFO mapreduce.Job: Job job_1479497522730_0001 running in uber mode : false
16/11/18 15:13:44 INFO mapreduce.Job:  map 0% reduce 0%
16/11/18 15:13:57 INFO mapreduce.Job:  map 15% reduce 0%
16/11/18 15:14:00 INFO mapreduce.Job:  map 24% reduce 0%
16/11/18 15:14:03 INFO mapreduce.Job:  map 33% reduce 0%
16/11/18 15:14:06 INFO mapreduce.Job:  map 42% reduce 0%
16/11/18 15:14:09 INFO mapreduce.Job:  map 48% reduce 0%
16/11/18 15:14:12 INFO mapreduce.Job:  map 55% reduce 0%
16/11/18 15:14:15 INFO mapreduce.Job:  map 56% reduce 0%
16/11/18 15:14:18 INFO mapreduce.Job:  map 58% reduce 0%
16/11/18 15:14:21 INFO mapreduce.Job:  map 59% reduce 0%
16/11/18 15:14:24 INFO mapreduce.Job:  map 60% reduce 0%
16/11/18 15:14:27 INFO mapreduce.Job:  map 61% reduce 0%
16/11/18 15:14:30 INFO mapreduce.Job:  map 63% reduce 0%
16/11/18 15:14:33 INFO mapreduce.Job:  map 65% reduce 0%
16/11/18 15:14:39 INFO mapreduce.Job:  map 67% reduce 0%
16/11/18 15:14:42 INFO mapreduce.Job:  map 68% reduce 0%
16/11/18 15:14:45 INFO mapreduce.Job:  map 69% reduce 0%
16/11/18 15:14:48 INFO mapreduce.Job:  map 71% reduce 0%
16/11/18 15:14:54 INFO mapreduce.Job:  map 73% reduce 0%
16/11/18 15:14:57 INFO mapreduce.Job:  map 74% reduce 0%
16/11/18 15:15:03 INFO mapreduce.Job:  map 77% reduce 0%
16/11/18 15:15:09 INFO mapreduce.Job:  map 80% reduce 0%
16/11/18 15:15:16 INFO mapreduce.Job:  map 81% reduce 0%
16/11/18 15:15:18 INFO mapreduce.Job:  map 82% reduce 0%
16/11/18 15:15:19 INFO mapreduce.Job:  map 83% reduce 0%
16/11/18 15:15:22 INFO mapreduce.Job:  map 84% reduce 0%
16/11/18 15:15:26 INFO mapreduce.Job:  map 85% reduce 0%
16/11/18 15:15:29 INFO mapreduce.Job:  map 87% reduce 0%
16/11/18 15:15:32 INFO mapreduce.Job:  map 90% reduce 0%
16/11/18 15:15:35 INFO mapreduce.Job:  map 91% reduce 0%
16/11/18 15:15:41 INFO mapreduce.Job:  map 93% reduce 0%
16/11/18 15:15:44 INFO mapreduce.Job:  map 94% reduce 0%
16/11/18 15:15:47 INFO mapreduce.Job:  map 96% reduce 0%
16/11/18 15:15:53 INFO mapreduce.Job:  map 98% reduce 0%
16/11/18 15:15:56 INFO mapreduce.Job:  map 100% reduce 0%
16/11/18 15:16:00 INFO mapreduce.Job: Job job_1479497522730_0001 completed successfully
16/11/18 15:16:00 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=238836
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=170
                HDFS: Number of bytes written=5120000000
                HDFS: Number of read operations=8
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=4
        Job Counters
                Launched map tasks=2
                Other local map tasks=2
                Total time spent by all maps in occupied slots (ms)=259513
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=259513
                Total vcore-seconds taken by all map tasks=259513
                Total megabyte-seconds taken by all map tasks=265741312
        Map-Reduce Framework
                Map input records=51200000
                Map output records=51200000
                Input split bytes=170
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=599
                CPU time spent (ms)=82100
                Physical memory (bytes) snapshot=315932672
                Virtual memory (bytes) snapshot=3119640576
                Total committed heap usage (bytes)=426246144
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=109963291816450258
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=5120000000

real    2m27.182s
user    0m6.185s
sys     0m0.732s

[hdfs@ip-172-31-56-113 ~]$ hdfs dfs -ls /user/bavaria/tgen512m
Found 3 items
-rw-r--r--   3 bavaria supergroup          0 2016-11-18 15:15 /user/bavaria/tgen512m/_SUCCESS
-rw-r--r--   3 bavaria supergroup 2560000000 2016-11-18 15:15 /user/bavaria/tgen512m/part-m-00000
-rw-r--r--   3 bavaria supergroup 2560000000 2016-11-18 15:15 /user/bavaria/tgen512m/part-m-00001


51200000 rows * 100 bytes =5120000000 bytes / 16777216 bytes (16mb) = around 305 blocks



```
