
<br>Start Cloudera Manager server agent</br>
<br><code>sudo service cloudera-scm-server start</code></br>
<br></br>
<br><code>
[centos@ip-172-31-14-158 ~]$ sudo head /var/log/cloudera-scm-server/cloudera-scm-server.log
2017-05-05 00:43:47,085 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.11.0 (#101 built by jenkins on 20170412-1255 git: 70cb1442626406432a6e7af5bdf206a384ca3f98)
</code></br>
<br>Add the complete line that contains the phrase "Started Jetty server"</br>
<br><code>
[centos@ip-172-31-14-158 ~]$ sudo cat /var/log/cloudera-scm-server/cloudera-scm-server.log | grep 'Started Jetty server'
2017-05-05 00:44:59,961 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
</code></br>
<br>Add the full contents of your db.properties file</br>
<br><code>
[centos@ip-172-31-14-158 ~]$ sudo cat /etc/cloudera-scm-server/db.properties
# Auto-generated by scm_prepare_database.sh on Fri May  5 00:35:29 UTC 2017
#
# For information describing how to configure the Cloudera Manager Server
# to connect to databases, see the "Cloudera Manager Installation Guide."
#
com.cloudera.cmf.db.type=mysql
com.cloudera.cmf.db.host=localhost
com.cloudera.cmf.db.name=hue
com.cloudera.cmf.db.user=hue
com.cloudera.cmf.db.setupType=EXTERNAL
com.cloudera.cmf.db.password=huepassword
</code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>
<br></br>
<br><code></code></br>