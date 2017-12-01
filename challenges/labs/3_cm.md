# Create users in HDFS

<code>[saturn@nodo3 ~]$ HADOOP_USER_NAME=hdfs hdfs dfs  -mkdir /user/saturn
[saturn@nodo3 ~]$ HADOOP_USER_NAME=hdfs hdfs dfs  -mkdir /user/haley
</code>


# Usuario hdfs dfs -ls /user

<code>
[haley@nodo3 ~]$ HADOOP_USER_NAME=hdfs hdfs dfs -ls /user
Found 7 items
drwxr-xr-x   - haley  supergroup          0 2017-12-01 18:15 /user/haley
drwxrwxrwx   - mapred hadoop              0 2017-12-01 17:53 /user/history
drwxrwxr-t   - hive   hive                0 2017-12-01 17:54 /user/hive
drwxrwxr-x   - hue    hue                 0 2017-12-01 17:55 /user/hue
drwxrwxr-x   - oozie  oozie               0 2017-12-01 17:55 /user/oozie
drwxr-xr-x   - saturn supergroup          0 2017-12-01 18:15 /user/saturn
drwxr-x--x   - spark  spark               0 2017-12-01 17:53 /user/spark

</code>
