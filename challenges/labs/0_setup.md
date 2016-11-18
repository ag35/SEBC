```
US N. Virginia
CentOS 6.5
ami-41ccea56

[root@ip-172-31-56-113 ~]# cat /etc/hosts
127.0.0.1               localhost.localdomain localhost
::1             localhost6.localdomain6 localhost6

172.31.56.113   ip-172-31-56-113.ec2.internal   ip-172-31-56-113.ec2    N1
172.31.56.114   ip-172-31-56-114.ec2.internal   ip-172-31-56-114.ec2    N2
172.31.56.115   ip-172-31-56-115.ec2.internal   ip-172-31-56-115.ec2    N3
172.31.56.116   ip-172-31-56-116.ec2.internal   ip-172-31-56-116.ec2    N4
172.31.56.117   ip-172-31-56-117.ec2.internal   ip-172-31-56-117.ec2    N5


N1
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        40G  713M   37G   2% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvdf        40G  176M   40G   1% /disks/disk1
N2
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        40G  702M   37G   2% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvdf        40G  176M   40G   1% /disks/disk1
N3
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        40G  702M   37G   2% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvdf        40G  176M   40G   1% /disks/disk1
N4
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        40G  702M   37G   2% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvdf        40G  176M   40G   1% /disks/disk1
N5
Filesystem      Size  Used Avail Use% Mounted on
/dev/xvde        40G  702M   37G   2% /
tmpfs           7.4G     0  7.4G   0% /dev/shm
/dev/xvdf        40G  176M   40G   1% /disks/disk1

[root@ip-172-31-56-113 ~]# yum repolist enabled
Loaded plugins: fastestmirror, presto
Determining fastest mirrors
 * base: mirrors.advancedhosters.com
 * extras: linux.cc.lehigh.edu
 * updates: mirror.cogentco.com
base                                                                               | 3.7 kB     00:00
extras                                                                             | 3.4 kB     00:00
updates                                                                            | 3.4 kB     00:00
updates/primary_db                                                                 | 3.1 MB     00:00
repo id                                     repo name                                               status
base                                        CentOS-6 - Base                                         6,696
extras                                      CentOS-6 - Extras                                          62
updates                                     CentOS-6 - Updates                                        603
repolist: 7,361


/etc/passwd
N1
bavaria:x:2500:2500::/home/bavaria:/bin/bash
saxony:x:2800:2800::/home/saxony:/bin/bash
N2
bavaria:x:2500:2500::/home/bavaria:/bin/bash
saxony:x:2800:2800::/home/saxony:/bin/bash
N3
bavaria:x:2500:2500::/home/bavaria:/bin/bash
saxony:x:2800:2800::/home/saxony:/bin/bash
N4
bavaria:x:2500:2500::/home/bavaria:/bin/bash
saxony:x:2800:2800::/home/saxony:/bin/bash
N5
bavaria:x:2500:2500::/home/bavaria:/bin/bash
saxony:x:2800:2800::/home/saxony:/bin/bash

/etc/group
N1
democratic:x:2801:saxony
social:x:2802:bavaria
N2
democratic:x:2801:saxony
social:x:2802:bavaria
N3
democratic:x:2801:saxony
social:x:2802:bavaria
N4
democratic:x:2801:saxony
social:x:2802:bavaria
N5
democratic:x:2801:saxony
social:x:2802:bavaria




