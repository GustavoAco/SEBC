#Server Log

2017-12-01 17:05:41,994 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -$


#status
[root@nodo2 ~]# service cloudera-scm-server status
/etc/init.d/cloudera-scm-server: line 109: pstree: command not found
● cloudera-scm-server.service - LSB: Cloudera SCM Server
   Loaded: loaded (/etc/rc.d/init.d/cloudera-scm-server; bad; vendor preset: disabled)
   Active: active (exited) since Fri 2017-12-01 17:05:46 UTC; 10min ago
     Docs: man:systemd-sysv-generator(8)
  Process: 1374 ExecStop=/etc/rc.d/init.d/cloudera-scm-server stop (code=exited, status=0/SUCCESS)
  Process: 1422 ExecStart=/etc/rc.d/init.d/cloudera-scm-server start (code=exited, status=0/SUCCESS)

Dec 01 17:05:41 nodo2.gus.com systemd[1]: Starting LSB: Cloudera SCM Server...
Dec 01 17:05:41 nodo2.gus.com cloudera-scm-server[1422]: /etc/rc.d/init.d/cloudera-scm-server: line 109: pstree: command not found
Dec 01 17:05:41 nodo2.gus.com su[1446]: (to cloudera-scm) root on none
Dec 01 17:05:46 nodo2.gus.com cloudera-scm-server[1422]: Starting cloudera-scm-server: [  OK  ]
Dec 01 17:05:46 nodo2.gus.com systemd[1]: Started LSB: Cloudera SCM Server.
[root@nodo2 ~]#


#db.properties

# The database name
com.cloudera.cmf.db.name=smc

# The database user
com.cloudera.cmf.db.user=cloudera

# The database user's password
com.cloudera.cmf.db.password=C@paCuatro1.

# The db setup type
# By default, it is set to INIT
# If scm-server uses Embedded DB then it is set to EMBEDDED
# If scm-server uses External DB then it is set to EXTERNAL
com.cloudera.cmf.db.setupType=EXTERNAL
