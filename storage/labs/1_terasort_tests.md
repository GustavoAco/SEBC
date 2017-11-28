[gustavoaco@nodo3 hadoop-0.20-mapreduce]$ [gustavoaco@nodo3 hadoop-0.20-mapreduce]$  hadoop jar hadoop-examples.jar teragen 100000000 /user/gustavoaco/terasort-inputt
17/11/28 23:00-bash: [gustavoaco@nodo3: command not found
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
                HDFS: Number of write operations=4
        Job Counters
                Launched map tasks=2
                Other local map tasks=2
                Total time spent by all maps in occupied slots (ms)=241421
                Total time spent by all reduces in occupied slots (ms)=0
-bash: 17/11/28: No such file or directory
                Total time spent by all map tasks (ms)=241421
                Total vcore-milliseconds taken by all map tasks=241421
                Total megabyte-milliseconds taken by all map tasks=247215104
        Map-Reduce Framework
                Map input records=100000000
[gustavoaco@nodo3 hadoop-0.20-mapreduce]$ 17/11/28 23:00:38 INFO mapreduce.JobSubmitter: number of splits:2
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=942
                CPU time spent (ms)=141900
                Physical memory (bytes) snapshot=469778432
                Virtual memory (bytes) snapshot=3179520000
                Total committed heap usage (bytes)=869793792
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=214760662691937609
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
-bash: 17/11/28: No such file or directory
                Bytes Written=10000000000
[gustavoaco@nodo3 hadoop-0.20-mapreduce]$ hadoop jar hadoop-examples.jar terasort /user/gustavoaco/terasort-input /user/gustavoaco/terasort-output
