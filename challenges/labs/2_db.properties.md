# Server Log

2017-12-01 17:05:41,994 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -$


# status
2017-12-01 17:06:24,615 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.


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
