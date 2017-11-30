 <h3>Versión API</h3>
<code>
 [root@node1 html]#curl -u admin:admin http://localhost:7180/api/version
v18
</code>
 <h3>Versión CM</h3>
 ```
 [root@node1 html]# curl -u admin:admin http://localhost:7180/api/v18/cm/version/
{
  "version" : "5.13.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20171002-1719",
  "gitHash" : "bd657e597e6743c458ee2c9aabe808b7c972981c",
  "snapshot" : false
}

 <h3>Versión CM</h3>
 
```
[root@node1 html]# curl -u admin:admin http://localhost:7180/api/v18/users
{
  "items" : [ {
    "name" : "GustavoAco",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}
```
<h3>Cm Bd</h3>
```
 curl -u admin:admin http://localhost:7180/api/v18/cm/scmDbInfo
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```
