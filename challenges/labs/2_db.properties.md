First Line log (cloudera-scm-server.log) :

2017-03-10 05:06:04,908 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.10.0 (#85 built by jenkins on 20170120-1037 git: aa0b5cd5eceaefe2f971c13ab657020d96bb842a)

Line that contains the phrase "Started Jetty server"
                [root@ip-192-168-0-209 cloudera-scm-server]# grep -n "Started Jetty server" cloudera-scm-server.log
                30815:2017-03-10 05:07:08,147 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
