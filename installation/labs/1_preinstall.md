 sysctl -a | grep vm.swappiness
vm.swappiness = 30
sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
sudo sysctl -p 
vm.swappiness = 1

mkfs.xfs -f /dev/sdd
mount -t xfs /dev/sdd /media/hhd2/


 nslookup node1g.cloudapp.net
Server:         168.63.129.16
Address:        168.63.129.16#53

Non-authoritative answer:
Name:   node1g.cloudapp.net
Address: 104.209.46.230
