# Cloud Provider
<center>AZURE</center>
#  IP address and DNS
    IP        DNS Name
10.0.0.10 nodo1.gus.com 
10.0.0.20 nodo2.gus.com 
10.0.0.30 nodo3.gus.com 
10.0.0.40 nodo4.gus.com 

# Linux Version

Red Hat 7.4

#Capacity Nodo1
```
[root@nodo1 cloudera]# df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda2        32G  1.6G   30G   5% /
devtmpfs         16G     0   16G   0% /dev
tmpfs            16G     0   16G   0% /dev/shm
tmpfs            16G  8.4M   16G   1% /run
tmpfs            16G     0   16G   0% /sys/fs/cgroup
/dev/sda1       497M  103M  394M  21% /boot
/dev/sdb1        63G  2.1G   58G   4% /mnt/resource
tmpfs           3.2G     0  3.2G   0% /run/user/1000
tmpfs           3.2G     0  3.2G   0% /run/user/0
/dev/sdc        128G   33M  128G   1% /mnt/hdd1
/dev/sdd        128G   33M  128G   1% /mnt/hdd2
```


 #yum repolist 
<code>
 [root@nodo1 cloudera]# yum repolist enabled
Loaded plugins: langpacks, product-id, search-disabled-repos
repo id                                                           repo na status
!rhui-microsoft-azure-rhel7                                       Microso      2
!rhui-rhel-7-server-dotnet-rhui-debug-rpms/7Server/x86_64         dotNET      27
!rhui-rhel-7-server-dotnet-rhui-rpms/7Server/x86_64               dotNET      63
!rhui-rhel-7-server-dotnet-rhui-source-rpms/7Server/x86_64        dotNET      32
!rhui-rhel-7-server-rhui-debug-rpms/7Server/x86_64                Red Hat  6,382
!rhui-rhel-7-server-rhui-extras-debug-rpms/x86_64                 Red Hat    126
!rhui-rhel-7-server-rhui-extras-rpms/x86_64                       Red Hat    709
!rhui-rhel-7-server-rhui-extras-source-rpms/x86_64                Red Hat    276
!rhui-rhel-7-server-rhui-optional-debug-rpms/7Server/x86_64       Red Hat  4,263
!rhui-rhel-7-server-rhui-optional-rpms/7Server/x86_64             Red Hat 13,030
!rhui-rhel-7-server-rhui-optional-source-rpms/7Server/x86_64      Red Hat  3,038
!rhui-rhel-7-server-rhui-rh-common-debug-rpms/7Server/x86_64      Red Hat     31
!rhui-rhel-7-server-rhui-rh-common-rpms/7Server/x86_64            Red Hat    228
!rhui-rhel-7-server-rhui-rh-common-source-rpms/7Server/x86_64     Red Hat     89
!rhui-rhel-7-server-rhui-rpms/7Server/x86_64                      Red Hat 17,720
!rhui-rhel-7-server-rhui-source-rpms/7Server/x86_64               Red Hat  5,185
!rhui-rhel-7-server-rhui-supplementary-debug-rpms/7Server/x86_64  Red Hat      0
!rhui-rhel-7-server-rhui-supplementary-rpms/7Server/x86_64        Red Hat    238
!rhui-rhel-7-server-rhui-supplementary-source-rpms/7Server/x86_64 Red Hat      8
!rhui-rhel-server-rhui-rhscl-7-debug-rpms/7Server/x86_64          Red Hat    570
!rhui-rhel-server-rhui-rhscl-7-rpms/7Server/x86_64                Red Hat  9,198
!rhui-rhel-server-rhui-rhscl-7-source-rpms/7Server/x86_64         Red Hat  3,841
repolist: 65,056
</code>


# add users
[root@nodo1 cloudera]# useradd -u 2800 saturn
[root@nodo1 cloudera]#  useradd -u 2900 haley

#Add user Group
[root@nodo1 cloudera]# usermod -a -G planets saturn
[root@nodo1 cloudera]# usermod -a -G comets saturn
# /etc/passwd
haley:x:2900:2900::/home/haley:/bin/bash
saturn:x:2800:2800::/home/saturn:/bin/bash

# /etcgroup
comets:x:2901:haley
planets:x:2902:saturn








