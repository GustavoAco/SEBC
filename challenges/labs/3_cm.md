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
# The command and output from the CM API call 
<code>
  {
  "items" : [ {
    "hostId" : "12a9bd29-6594-481b-8884-d05d2a6fa985",
    "ipAddress" : "10.0.0.10",
    "hostname" : "nodo1.gus.com",
    "rackId" : "/default",
    "hostUrl" : "http://nodo2.gus.com:7180/cmf/hostRedirect/12a9bd29-6594-481b-8884-d05d2a6fa985",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 33722032128
  }, {
    "hostId" : "3860e363-9d8f-46b9-9800-a2a691e02707",
    "ipAddress" : "10.0.0.20",
    "hostname" : "nodo2.gus.com",
    "rackId" : "/default",
    "hostUrl" : "http://nodo2.gus.com:7180/cmf/hostRedirect/3860e363-9d8f-46b9-9800-a2a691e02707",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 33722032128
  }, {
    "hostId" : "13d6e524-5ce2-42f6-aced-788a163f8550",
    "ipAddress" : "10.0.0.30",
    "hostname" : "nodo3.gus.com",
    "rackId" : "/default",
    "hostUrl" : "http://nodo2.gus.com:7180/cmf/hostRedirect/13d6e524-5ce2-42f6-aced-788a163f8550",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 33722032128
  }, {
    "hostId" : "aa3a8c23-963c-4d7a-a7cf-a02707d4ad52",
    "ipAddress" : "10.0.0.40",
    "hostname" : "nodo4.gus.com",
    "rackId" : "/default",
    "hostUrl" : "http://nodo2.gus.com:7180/cmf/hostRedirect/aa3a8c23-963c-4d7a-a7cf-a02707d4ad52",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 8,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 33722032128
  } ]
}
</code>

# The command and output from the CM API call ../api/v8/clusters/<githubName>/services

<code>
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://nodo2.gus.com:7180/cmf/serviceRedirect/hive",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://nodo2.gus.com:7180/cmf/serviceRedirect/zookeeper",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://nodo2.gus.com:7180/cmf/serviceRedirect/hue",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://nodo2.gus.com:7180/cmf/serviceRedirect/oozie",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://nodo2.gus.com:7180/cmf/serviceRedirect/yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)"
  }, {
    "name" : "spark_on_yarn",
    "type" : "SPARK_ON_YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://nodo2.gus.com:7180/cmf/serviceRedirect/spark_on_yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Spark"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://nodo2.gus.com:7180/cmf/serviceRedirect/hdfs",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "DISABLED"
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS"
  } ]
}
</code>
