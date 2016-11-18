```
[saxony@ip-172-31-56-113 ~]$ hadoop jar /opt/cloudera/parcels/CDH-5.7.5-1.cdh5.7.5.p0.3/lib/hadoop-0.20-mapreduce/hadoop-examples.jar pi 1 1000
Number of Maps  = 1
Samples per Map = 1000
Wrote input for Map #0
Starting Job
16/11/18 15:38:48 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-56-113.ec2.internal/172.31.56.113:8032
16/11/18 15:38:48 INFO hdfs.DFSClient: Created token for saxony: HDFS_DELEGATION_TOKEN owner=saxony@AG35.IL, renewer=yarn, realUser=, issueDate=1479501528472, maxDate=1480106328472, sequenceNumber=2, masterKeyId=2 on 172.31.56.113:8020
16/11/18 15:38:48 INFO security.TokenCache: Got dt for hdfs://ip-172-31-56-113.ec2.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.56.113:8020, Ident: (token for saxony: HDFS_DELEGATION_TOKEN owner=saxony@AG35.IL, renewer=yarn, realUser=, issueDate=1479501528472, maxDate=1480106328472, sequenceNumber=2, masterKeyId=2)
16/11/18 15:38:48 INFO input.FileInputFormat: Total input paths to process : 1
16/11/18 15:38:48 INFO mapreduce.JobSubmitter: number of splits:1
16/11/18 15:38:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1479500950411_0002
16/11/18 15:38:49 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.56.113:8020, Ident: (token for saxony: HDFS_DELEGATION_TOKEN owner=saxony@AG35.IL, renewer=yarn, realUser=, issueDate=1479501528472, maxDate=1480106328472, sequenceNumber=2, masterKeyId=2)
16/11/18 15:38:49 INFO impl.YarnClientImpl: Submitted application application_1479500950411_0002
16/11/18 15:38:49 INFO mapreduce.Job: The url to track the job: http://ip-172-31-56-113.ec2.internal:8088/proxy/application_1479500950411_0002/
16/11/18 15:38:49 INFO mapreduce.Job: Running job: job_1479500950411_0002
16/11/18 15:39:03 INFO mapreduce.Job: Job job_1479500950411_0002 running in uber mode : false
16/11/18 15:39:03 INFO mapreduce.Job:  map 0% reduce 0%
16/11/18 15:39:16 INFO mapreduce.Job:  map 100% reduce 0%
16/11/18 15:39:27 INFO mapreduce.Job:  map 100% reduce 100%
16/11/18 15:39:27 INFO mapreduce.Job: Job job_1479500950411_0002 completed successfully
16/11/18 15:39:27 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=38
                FILE: Number of bytes written=241655
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=285
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=7
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=1
                Launched reduce tasks=1
                Data-local map tasks=1
                Total time spent by all maps in occupied slots (ms)=8758
                Total time spent by all reduces in occupied slots (ms)=4871
                Total time spent by all map tasks (ms)=8758
                Total time spent by all reduce tasks (ms)=4871
                Total vcore-seconds taken by all map tasks=8758
                Total vcore-seconds taken by all reduce tasks=4871
                Total megabyte-seconds taken by all map tasks=8968192
                Total megabyte-seconds taken by all reduce tasks=4987904
        Map-Reduce Framework
                Map input records=1
                Map output records=2
                Map output bytes=18
                Map output materialized bytes=34
                Input split bytes=167
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=34
                Reduce input records=2
                Reduce output records=0
                Spilled Records=4
                Shuffled Maps =1
                Failed Shuffles=0
                Merged Map outputs=1
                GC time elapsed (ms)=79
                CPU time spent (ms)=2100
                Physical memory (bytes) snapshot=630964224
                Virtual memory (bytes) snapshot=3145154560
                Total committed heap usage (bytes)=740818944
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=118
        File Output Format Counters
                Bytes Written=97
Job Finished in 39.311 seconds
Estimated value of Pi is 3.14800000000000000000
```