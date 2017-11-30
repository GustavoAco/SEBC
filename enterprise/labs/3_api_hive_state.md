```
[root@node1 ~]# curl -X POST -u admin:admin 'http://localhost:7180/api/v1/clusters/GustavoAco/services/hive/commands/stop'
{
  "id" : 349,
  "name" : "Stop",
  "startTime" : "2017-11-30T20:00:19.358Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}[root@node1 ~]# curl -X POST -u admin:admin 'http://localhost:7180/api/v1/clusters/GustavoAco/services/hive/commands/start'
{
  "id" : 355,
  "name" : "Start",
  "startTime" : "2017-11-30T20:01:38.820Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}

```
