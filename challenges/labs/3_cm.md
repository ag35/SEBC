```
mysql> show grants for rman;
+-----------------------------------------------------------------------------------------------------+
| Grants for rman@%                                                                                   |
+-----------------------------------------------------------------------------------------------------+
| GRANT USAGE ON *.* TO 'rman'@'%' IDENTIFIED BY PASSWORD '*819397F8B454D58DA4E9F42A88A4873756B8C96D' |
| GRANT ALL PRIVILEGES ON `rman`.* TO 'rman'@'%'                                                      |
+-----------------------------------------------------------------------------------------------------+
2 rows in set (0.00 sec)

mysql> show grants for hive;
+-----------------------------------------------------------------------------------------------------+
| Grants for hive@%                                                                                   |
+-----------------------------------------------------------------------------------------------------+
| GRANT USAGE ON *.* TO 'hive'@'%' IDENTIFIED BY PASSWORD '*4DF1D66463C18D44E3B001A8FB1BBFBEA13E27FC' |
| GRANT ALL PRIVILEGES ON `hive`.* TO 'hive'@'%'                                                      |
+-----------------------------------------------------------------------------------------------------+
2 rows in set (0.00 sec)

mysql> show grants for scm;
ERROR 1141 (42000): There is no such grant defined for user 'scm' on host '%'
^^^^^^^^^^^^ - this is expected, here is the correct grant:

mysql> show grants for scm@'ip-172-31-56-114.ec2.internal';
+--------------------------------------------------------------------------------------------------------------------------------+
| Grants for scm@ip-172-31-56-114.ec2.internal                                                                                   |
+--------------------------------------------------------------------------------------------------------------------------------+
| GRANT USAGE ON *.* TO 'scm'@'ip-172-31-56-114.ec2.internal' IDENTIFIED BY PASSWORD '*45E6E3C68BDF1AC7EBB5C5A3BCBD5E9437B293BE' |
| GRANT ALL PRIVILEGES ON `scm`.* TO 'scm'@'ip-172-31-56-114.ec2.internal'                                                       |
+--------------------------------------------------------------------------------------------------------------------------------+
2 rows in set (0.00 sec)

[hdfs@ip-172-31-56-113 ~]$ hdfs dfs -ls /user
Found 8 items
drwxr-xr-x   - admin   admin               0 2016-11-18 14:12 /user/admin
drwxr-xr-x   - bavaria supergroup          0 2016-11-18 14:34 /user/bavaria
drwxr-xr-x   - hdfs    supergroup          0 2016-11-18 14:12 /user/hdfs
drwxrwxrwx   - mapred  hadoop              0 2016-11-18 14:07 /user/history
drwxrwxr-t   - hive    hive                0 2016-11-18 14:08 /user/hive
drwxrwxr-x   - hue     hue                 0 2016-11-18 14:09 /user/hue
drwxrwxr-x   - oozie   oozie               0 2016-11-18 14:09 /user/oozie
drwxr-xr-x   - saxony  supergroup          0 2016-11-18 14:34 /user/saxony
[hdfs@ip-172-31-56-113 ~]$


{
  "items" : [ {
    "hostId" : "i-0f5d000fb225f3988",
    "ipAddress" : "172.31.56.113",
    "hostname" : "ip-172-31-56-113.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-56-114.ec2.internal:7180/cmf/hostRedirect/i-0f5d000fb225f3988",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-09d9fa9c137cfe48e",
    "ipAddress" : "172.31.56.114",
    "hostname" : "ip-172-31-56-114.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-56-114.ec2.internal:7180/cmf/hostRedirect/i-09d9fa9c137cfe48e",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-00228729c06f07667",
    "ipAddress" : "172.31.56.115",
    "hostname" : "ip-172-31-56-115.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-56-114.ec2.internal:7180/cmf/hostRedirect/i-00228729c06f07667",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-0063ddc3605c5e9c5",
    "ipAddress" : "172.31.56.116",
    "hostname" : "ip-172-31-56-116.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-56-114.ec2.internal:7180/cmf/hostRedirect/i-0063ddc3605c5e9c5",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  }, {
    "hostId" : "i-0738d8c6160a33c17",
    "ipAddress" : "172.31.56.117",
    "hostname" : "ip-172-31-56-117.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-56-114.ec2.internal:7180/cmf/hostRedirect/i-0738d8c6160a33c17",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 15740305408
  } ]
}

```