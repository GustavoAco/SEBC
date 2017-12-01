# time
Testing loop ended on Fri Dec 1 19:35:07 UTC 2017


# teragen
<code>
hadoop jar hadoop-examples.jar teragen -D dfs.block.size=33554432 536870912  /user/saturn/terg
java.io.IOException: Output directory /user/saturn/terg already exists.
        at org.apache.hadoop.examples.terasort.TeraGen.run(TeraGen.java:293)
        at org.apache.hadoop.util.ToolRunner.run(ToolRunner.java:70)
        at org.apache.hadoop.examples.terasort.TeraGen.main(TeraGen.java:309)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.ProgramDriver$ProgramDescription.invoke(ProgramDriver.java:71)
        at org.apache.hadoop.util.ProgramDriver.run(ProgramDriver.java:144)
        at org.apache.hadoop.examples.ExampleDriver.main(ExampleDriver.java:74)
        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
        at java.lang.reflect.Method.invoke(Method.java:606)
        at org.apache.hadoop.util.RunJar.run(RunJar.java:221)
        at org.apache.hadoop.util.RunJar.main(RunJar.java:136)
[saturn@nodo3 lib]$ HADOOP_USER_NAME=hdfs hdfs dfs -rm /user/saturn/terag
rm: `/user/saturn/terag': No such file or directory
[saturn@nodo3 lib]$ HADOOP_USER_NAME=hdfs hdfs dfs -rm -R /user/saturn/terag
rm: `/user/saturn/terag': No such file or directory
[saturn@nodo3 lib]$ HADOOP_USER_NAME=hdfs hdfs dfs -rmr /user/saturn/terag
rmr: DEPRECATED: Please use 'rm -r' instead.
rmr: `/user/saturn/terag': No such file or directory
[saturn@nodo3 lib]$ HADOOP_USER_NAME=hdfs hdfs dfs -rm -r /user/saturn/terag/
rm: `/user/saturn/terag/': No such file or directory
[saturn@nodo3 lib]$ hadoop jar hadoop-examples.jar teragen -D dfs.block.size=33554432 536870912  /user/saturn/terga
17/12/01 19:51:21 INFO client.RMProxy: Connecting to ResourceManager at nodo3.gus.com/10.0.0.30:8032
17/12/01 19:51:24 INFO terasort.TeraSort: Generating 536870912 using 2
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: number of splits:2
17/12/01 19:51:24 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1512151823991_0005
17/12/01 19:51:24 INFO impl.YarnClientImpl: Submitted application application_1512151823991_0005
17/12/01 19:51:24 INFO mapreduce.Job: The url to track the job: http://nodo3.gus.com:8088/proxy/application_1512151823991_0005/
17/12/01 19:51:24 INFO mapreduce.Job: Running job: job_1512151823991_0005
17/12/01 19:51:44 INFO mapreduce.Job: Job job_1512151823991_0005 running in uber mode : false
17/12/01 19:51:44 INFO mapreduce.Job:  map 0% reduce 0%
17/12/01 19:52:03 INFO mapreduce.Job:  map 1% reduce 0%
17/12/01 19:52:06 INFO mapreduce.Job:  map 2% reduce 0%
17/12/01 19:52:09 INFO mapreduce.Job:  map 3% reduce 0%
 hadoop jar hadoop-examples.jar teragen -D dfs.block.size=33554432 536870912  /user/saturn/terga
17/12/01 19:51:21 INFO client.RMProxy: Connecting to ResourceManager at nodo3.gus.com/10.0.0.30:8032
17/12/01 19:51:24 INFO terasort.TeraSort: Generating 536870912 using 2
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: number of splits:2
17/12/01 19:51:24 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1512151823991_0005
17/12/01 19:51:24 INFO impl.YarnClientImpl: Submitted application application_1512151823991_0005
17/12/01 19:51:24 INFO mapreduce.Job: The url to track the job: http://nodo3.gus.com:8088/proxy/application_1512151823991_0005/
17/12/01 19:51:24 INFO mapreduce.Job: Running job: job_1512151823991_0005
17/12/01 19:51:44 INFO mapreduce.Job: Job job_1512151823991_0005 running in uber mode : false
17/12/01 19:51:44 INFO mapreduce.Job:  map 0% reduce 0%
17/12/01 19:52:03 INFO mapreduce.Job:  map 1% reduce 0%
17/12/01 19:52:06 INFO mapreduce.Job:  map 2% reduce 0%
hadoop jar hadoop-examples.jar teragen -D dfs.block.size=33554432 536870912  /user/saturn/terga
17/12/01 19:51:21 INFO client.RMProxy: Connecting to ResourceManager at nodo3.gus.com/10.0.0.30:8032
17/12/01 19:51:24 INFO terasort.TeraSort: Generating 536870912 using 2
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: number of splits:2
17/12/01 19:51:24 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1512151823991_0005
17/12/01 19:51:24 INFO impl.YarnClientImpl: Submitted application application_1512151823991_0005
17/12/01 19:51:24 INFO mapreduce.Job: The url to track the job: http://nodo3.gus.com:8088/proxy/application_1512151823991_0005/
17/12/01 19:51:24 INFO mapreduce.Job: Running job: job_1512151823991_0005
17/12/01 19:51:44 INFO mapreduce.Job: Job job_1512151823991_0005 running in uber mode : false
17/12/01 19:51:44 INFO mapreduce.Job:  map 0% reduce 0%
17/12/01 19:52:03 INFO mapreduce.Job:  map 1% reduce 0%
17/12/01 19:52:06 INFO mapreduce.Job:  map 2% reduce 0%
17/12/01 19:52:09 INFO mapreduce.Job:  map 3% reduce 0%
 hadoop jar hadoop-examples.jar teragen -D dfs.block.size=33554432 536870912  /user/saturn/terga
17/12/01 19:51:21 INFO client.RMProxy: Connecting to ResourceManager at nodo3.gus.com/10.0.0.30:8032
17/12/01 19:51:24 INFO terasort.TeraSort: Generating 536870912 using 2
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: number of splits:2
17/12/01 19:51:24 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/12/01 19:51:24 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1512151823991_0005
17/12/01 19:51:24 INFO impl.YarnClientImpl: Submitted application application_1512151823991_0005
17/12/01 19:51:24 INFO mapreduce.Job: The url to track the job: http://nodo3.gus.com:8088/proxy/application_1512151823991_0005/
17/12/01 19:51:24 INFO mapreduce.Job: Running job: job_1512151823991_0005
17/12/01 19:51:44 INFO mapreduce.Job: Job job_1512151823991_0005 running in uber mode : false
17/12/01 19:51:44 INFO mapreduce.Job:  map 0% reduce 0%
17/12/01 19:52:27 INFO mapreduce.Job:  map 4% reduce 0%
17/12/01 19:52:42 INFO mapreduce.Job:  map 5% reduce 0%
17/12/01 19:52:54 INFO mapreduce.Job:  map 7% reduce 0%
17/12/01 19:53:09 INFO mapreduce.Job:  map 8% reduce 0%
17/12/01 19:53:12 INFO mapreduce.Job:  map 9% reduce 0%
17/12/01 19:53:21 INFO mapreduce.Job:  map 10% reduce 0%
17/12/01 19:53:24 INFO mapreduce.Job:  map 11% reduce 0%
17/12/01 19:53:45 INFO mapreduce.Job:  map 12% reduce 0%
17/12/01 19:53:48 INFO mapreduce.Job:  map 13% reduce 0%
17/12/01 19:53:54 INFO mapreduce.Job:  map 14% reduce 0%
17/12/01 19:53:57 INFO mapreduce.Job:  map 15% reduce 0%
17/12/01 19:54:00 INFO mapreduce.Job:  map 16% reduce 0%
17/12/01 19:54:03 INFO mapreduce.Job:  map 17% reduce 0%
17/12/01 19:54:06 INFO mapreduce.Job:  map 18% reduce 0%
17/12/01 19:54:09 INFO mapreduce.Job:  map 19% reduce 0%
17/12/01 19:54:12 INFO mapreduce.Job:  map 20% reduce 0%
17/12/01 19:54:19 INFO mapreduce.Job:  map 21% reduce 0%
17/12/01 19:54:22 INFO mapreduce.Job:  map 22% reduce 0%
^C^C^C^C^C^C^C^C^C^C^C^C^C^C^C^C^C^C^C^C[saturn@nodo3 lib]$
[saturn@nodo3 lib]$ HADOOP_USER_NAME=hdfs hadoop jar hadoop-examples.jar teragen -D dfs.block.size=33554432 -D mapreduce.job.maps=12 65536000 /user/saturn/results/tgen
17/12/01 19:55:08 INFO client.RMProxy: Connecting to ResourceManager at nodo3.gus.com/10.0.0.30:8032
17/12/01 19:55:09 INFO terasort.TeraSort: Generating 65536000 using 12
17/12/01 19:55:09 INFO mapreduce.JobSubmitter: number of splits:12
17/12/01 19:55:09 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/12/01 19:55:09 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1512151823991_0006
17/12/01 19:55:10 INFO impl.YarnClientImpl: Submitted application application_1512151823991_0006
17/12/01 19:55:10 INFO mapreduce.Job: The url to track the job: http://nodo3.gus.com:8088/proxy/application_1512151823991_0006/
17/12/01 19:55:10 INFO mapreduce.Job: Running job: job_1512151823991_0006
17/12/01 19:55:17 INFO mapreduce.Job: Job job_1512151823991_0006 running in uber mode : false
17/12/01 19:55:17 INFO mapreduce.Job:  map 0% reduce 0%
17/12/01 19:55:37 INFO mapreduce.Job:  map 9% reduce 0%
17/12/01 19:55:38 INFO mapreduce.Job:  map 16% reduce 0%
17/12/01 19:55:39 INFO mapreduce.Job:  map 19% reduce 0%
17/12/01 19:55:40 INFO mapreduce.Job:  map 23% reduce 0%
17/12/01 19:55:42 INFO mapreduce.Job:  map 24% reduce 0%
17/12/01 19:55:43 INFO mapreduce.Job:  map 25% reduce 0%
17/12/01 19:55:54 INFO mapreduce.Job:  map 27% reduce 0%
17/12/01 19:55:55 INFO mapreduce.Job:  map 45% reduce 0%
17/12/01 19:55:56 INFO mapreduce.Job:  map 50% reduce 0%
17/12/01 19:56:05 INFO mapreduce.Job:  map 52% reduce 0%
17/12/01 19:56:06 INFO mapreduce.Job:  map 53% reduce 0%
17/12/01 19:56:07 INFO mapreduce.Job:  map 78% reduce 0%
17/12/01 19:56:09 INFO mapreduce.Job:  map 79% reduce 0%
17/12/01 19:56:10 INFO mapreduce.Job:  map 85% reduce 0%
17/12/01 19:56:13 INFO mapreduce.Job:  map 87% reduce 0%
17/12/01 19:56:17 INFO mapreduce.Job:  map 88% reduce 0%
17/12/01 19:56:31 INFO mapreduce.Job:  map 92% reduce 0%
17/12/01 19:56:33 INFO mapreduce.Job:  map 95% reduce 0%
17/12/01 19:56:34 INFO mapreduce.Job:  map 100% reduce 0%
17/12/01 19:56:35 INFO mapreduce.Job: Job job_1512151823991_0006 completed successfully
17/12/01 19:56:35 INFO mapreduce.Job: Counters: 31
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=1469402
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=1025
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=48
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=24
        Job Counters
                Launched map tasks=12
                Other local map tasks=12
                Total time spent by all maps in occupied slots (ms)=803502
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=803502
                Total vcore-seconds taken by all map tasks=803502
                Total megabyte-seconds taken by all map tasks=822786048
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=1025
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=3233
                CPU time spent (ms)=181790
                Physical memory (bytes) snapshot=4318355456
                Virtual memory (bytes) snapshot=19261767680
                Total committed heap usage (bytes)=6992953344
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

</code>

