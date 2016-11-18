```
[root@ip-172-31-56-114 yum.repos.d]# ls -lrt
total 28
-rw-r--r--. 1 root root 3664 Nov 27  2013 CentOS-Vault.repo
-rw-r--r--. 1 root root  630 Nov 27  2013 CentOS-Media.repo
-rw-r--r--. 1 root root  638 Nov 27  2013 CentOS-Debuginfo.repo
-rw-r--r--. 1 root root 1926 Nov 27  2013 CentOS-Base.repo
-rw-r--r--  1 root root 1440 Sep 12 06:32 mysql-community-source.repo
-rw-r--r--  1 root root 1414 Nov 18 12:56 mysql-community.repo
-rw-r--r--  1 root root  294 Nov 18 13:16 cloudera-manager.repo

grant all on scm.* to 'scm'@'ip-172-31-56-114.ec2.internal' ;

[root@ip-172-31-56-114 yum.repos.d]# /usr/share/cmf/schema/scm_prepare_database.sh mysql scm scm scm -h ip-172-31-56-113.ec2.internal
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/java/jdk1.7.0_67-cloudera/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
2016-11-18 13:30:34,848 [main] INFO  com.cloudera.enterprise.dbutil.DbCommandExecutor  - Successfully connected to database.
All done, your SCM database is configured correctly!


```