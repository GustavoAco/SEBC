# List repos nodo2

[root@nodo2 nodo2]# ls /etc/yum.repos.d/
mysql-community.repo  mysql-community-source.repo  redhat.repo  rh-cloud.repo

 --adding cloudera repo in file cloudera.repo
 
[root@nodo2 nodo2]# ls /etc/yum.repos.d/                                        cloudera.repo         mysql-community-source.repo  rh-cloud.repo
mysql-community.repo  redhat.repo

/usr/share/cmf/schema/scm_prepare_database.sh mysql scm cloudera C@paCuatro1.

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




