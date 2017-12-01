<h3>Terasort</h3>
 <strong><code>hadoop jar hadoop-examples.jar teragen 100000000 /user/gustavoaco/terasort-input</code> </strong>
 <br>
 <code>
 [gustavoaco@nodo3 hadoop-0.20-mapreduce]$  hadoop jar hadoop-examples.jar teragen 100000000 /user/gustavoaco/terasort-input
:38 INFO terasort.TeraGen: Generating 100000000 using 2
17/11/28 23:00:38 INFO mapreduce.JobSubmitter: number of splits:2
17/11/28 23:00:38 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511905996400_0002
17/11/28 23:00:39 INFO impl.YarnClientImpl: Submitted application application_1511905996400_0002
17/11/28 23:00:39 INFO mapreduce.Job: The url to track the job: http://nodo2.nodo2gus.d3.internal.cloudapp.net:8088/proxy/application_1511905996400_0002/
17/11/28 23:00:39 INFO mapreduce.Job: Running job: job_1511905996400_0002
17/11/28 23:00:45 INFO mapreduce.Job: Job job_1511905996400_0002 running in uber mode : false
17/11/28 23:00:45 INFO mapreduce.Job:  map 0% reduce 0%
[gustavoaco@nodo3 hadoop-0.20-mapreduce]$ 17/11/28 23:00:38 INFO client.RMProxy: Connecting to ResourceManager at nodo2.nodo2gus.d3.internal.cloudapp.net/10.0.0.20:8032
17/11/28 23:01:03 INFO mapreduce.Job:  map 15% reduce 0%
17/11/28 23:01:09 INFO mapreduce.Job:  map 19% reduce 0%
17/11/28 23:01:15 INFO mapreduce.Job:  map 23% reduce 0%
17/11/28 23:01:21 INFO mapreduce.Job:  map 33% reduce 0%
17/11/28 23:01:27 INFO mapreduce.Job:  map 40% reduce 0%
17/11/28 23:01:45 INFO mapreduce.Job:  map 43% reduce 0%
17/11/28 23:01:51 INFO mapreduc-bash: 17/11/28: No such file or directory
e.Job:  map 48% reduce 0%
17/11/28 23:01:57 INFO mapreduce.Job:  map 58% reduce 0%
17/11/28 23:02:03 INFO mapreduce.Job:  map 62% reduce 0%
17/11/28 23:02:09 INFO mapreduce.Job:  map 65% reduce 0%
17/11/28 23:02:15 INFO mapreduce.Job:  map 76% reduce 0%
[gustavoaco@nodo3 hadoop-0.20-mapreduce]$ 17/11/28 23:00:38 INFO terasort.TeraGen: Generating 100000000 using 2
                HDFS: Number of large read operations=0
 </code>
 <h3>Terasort/h3>
 <strong><code>hadoop jar hadoop-examples.jar terasort /user/gustavoaco/terasort-input /user/gustavoaco/terasort-output</code> </strong>
 <br>
 <code>
[gustavoaco@nodo3 hadoop-0.20-mapreduce]$ hadoop jar hadoop-examples.jar terasort /user/gustavoaco/terasort-input /user/gustavoaco/terasort-output
17/11/28 23:18:06 INFO terasort.TeraSort: starting
17/11/28 23:18:07 INFO input.FileInputFormat: Total input paths to process : 2
Spent 182ms computing base-splits.
Spent 3ms computing TeraScheduler splits.
Computing input splits took 186ms
Sampling 10 splits of 76
Making 12 from 100000 sampled records
Computing parititions took 620ms
Spent 809ms computing partitions.
17/11/28 23:18:08 INFO client.RMProxy: Connecting to ResourceManager at nodo2.nodo2gus.d3.internal.cloudapp.net/10.0.0.20:8032
17/11/28 23:18:08 INFO mapreduce.JobSubmitter: number of splits:76
17/11/28 23:18:08 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1511905996400_0003
17/11/28 23:18:09 INFO impl.YarnClientImpl: Submitted application application_1511905996400_0003
17/11/28 23:18:09 INFO mapreduce.Job: The url to track the job: http://nodo2.nodo2gus.d3.internal.cloudapp.net:8088/proxy/application_1511905996400_0003/
17/11/28 23:18:09 INFO mapreduce.Job: Running job: job_1511905996400_0003
17/11/28 23:18:15 INFO mapreduce.Job: Job job_1511905996400_0003 running in uber mode : false
17/11/28 23:18:15 INFO mapreduce.Job:  map 0% reduce 0%
17/11/28 23:18:27 INFO mapreduce.Job:  map 4% reduce 0%
17/11/28 23:18:28 INFO mapreduce.Job:  map 5% reduce 0%
17/11/28 23:18:29 INFO mapreduce.Job:  map 9% reduce 0%
17/11/28 23:18:30 INFO mapreduce.Job:  map 11% reduce 0%
17/11/28 23:18:31 INFO mapreduce.Job:  map 12% reduce 0%
17/11/28 23:18:35 INFO mapreduce.Job:  map 18% reduce 0%
17/11/28 23:18:36 INFO mapreduce.Job:  map 22% reduce 0%
17/11/28 23:18:38 INFO mapreduce.Job:  map 28% reduce 0%
17/11/28 23:18:42 INFO mapreduce.Job:  map 32% reduce 0%
17/11/28 23:18:43 INFO mapreduce.Job:  map 34% reduce 0%
17/11/28 23:18:49 INFO mapreduce.Job:  map 39% reduce 0%
17/11/28 23:18:52 INFO mapreduce.Job:  map 41% reduce 0%
17/11/28 23:18:53 INFO mapreduce.Job:  map 46% reduce 0%
17/11/28 23:18:54 INFO mapreduce.Job:  map 51% reduce 0%
17/11/28 23:18:55 INFO mapreduce.Job:  map 54% reduce 0%
17/11/28 23:18:56 INFO mapreduce.Job:  map 57% reduce 0%
17/11/28 23:18:59 INFO mapreduce.Job:  map 59% reduce 0%
17/11/28 23:19:00 INFO mapreduce.Job:  map 62% reduce 0%
17/11/28 23:19:08 INFO mapreduce.Job:  map 64% reduce 0%
17/11/28 23:19:09 INFO mapreduce.Job:  map 68% reduce 0%
17/11/28 23:19:10 INFO mapreduce.Job:  map 82% reduce 0%
17/11/28 23:19:11 INFO mapreduce.Job:  map 84% reduce 0%
17/11/28 23:19:17 INFO mapreduce.Job:  map 86% reduce 0%
17/11/28 23:19:21 INFO mapreduce.Job:  map 91% reduce 0%
17/11/28 23:19:22 INFO mapreduce.Job:  map 96% reduce 0%
17/11/28 23:19:25 INFO mapreduce.Job:  map 100% reduce 0%
17/11/28 23:19:29 INFO mapreduce.Job:  map 100% reduce 6%
17/11/28 23:19:32 INFO mapreduce.Job:  map 100% reduce 8%
17/11/28 23:19:33 INFO mapreduce.Job:  map 100% reduce 23%
17/11/28 23:19:35 INFO mapreduce.Job:  map 100% reduce 24%
17/11/28 23:19:38 INFO mapreduce.Job:  map 100% reduce 50%
17/11/28 23:19:39 INFO mapreduce.Job:  map 100% reduce 67%
17/11/28 23:19:40 INFO mapreduce.Job:  map 100% reduce 73%
17/11/28 23:19:41 INFO mapreduce.Job:  map 100% reduce 74%
17/11/28 23:19:44 INFO mapreduce.Job:  map 100% reduce 78%
17/11/28 23:19:45 INFO mapreduce.Job:  map 100% reduce 80%
17/11/28 23:19:46 INFO mapreduce.Job:  map 100% reduce 81%
17/11/28 23:19:51 INFO mapreduce.Job:  map 100% reduce 83%
17/11/28 23:19:58 INFO mapreduce.Job:  map 100% reduce 85%
17/11/28 23:20:00 INFO mapreduce.Job:  map 100% reduce 86%
17/11/28 23:20:02 INFO mapreduce.Job:  map 100% reduce 87%
17/11/28 23:20:04 INFO mapreduce.Job:  map 100% reduce 95%
17/11/28 23:20:08 INFO mapreduce.Job:  map 100% reduce 98%
17/11/28 23:20:10 INFO mapreduce.Job:  map 100% reduce 99%
17/11/28 23:20:25 INFO mapreduce.Job:  map 100% reduce 100%
17/11/28 23:20:27 INFO mapreduce.Job: Job job_1511905996400_0003 completed successfully
17/11/28 23:20:27 INFO mapreduce.Job: Counters: 49
        File System Counters
                FILE: Number of bytes read=4442784183
                FILE: Number of bytes written=8826611038
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=10000012160
                HDFS: Number of bytes written=10000000000
                HDFS: Number of read operations=264
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=24
        Job Counters
                Launched map tasks=76
                Launched reduce tasks=12
                Data-local map tasks=76
                Total time spent by all maps in occupied slots (ms)=967395
                Total time spent by all reduces in occupied slots (ms)=631647
                Total time spent by all map tasks (ms)=967395
                Total time spent by all reduce tasks (ms)=631647
                Total vcore-milliseconds taken by all map tasks=967395
                Total vcore-milliseconds taken by all reduce tasks=631647
                Total megabyte-milliseconds taken by all map tasks=990612480
                Total megabyte-milliseconds taken by all reduce tasks=646806528
        Map-Reduce Framework
                Map input records=100000000
                Map output records=100000000
                Map output bytes=10200000000
                Map output materialized bytes=4370860826
                Input split bytes=12160
                Combine input records=0
                Combine output records=0
                Reduce input groups=100000000
                Reduce shuffle bytes=4370860826
                Reduce input records=100000000
                Reduce output records=100000000
                Spilled Records=200000000
                Shuffled Maps =912
                Failed Shuffles=0
                Merged Map outputs=912
                GC time elapsed (ms)=17698
                CPU time spent (ms)=964610
                Physical memory (bytes) snapshot=57618669568
                Virtual memory (bytes) snapshot=141021614080
                Total committed heap usage (bytes)=55877566464
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
17/11/28 23:20:27 INFO terasort.TeraSort: done
</code>
