 sysctl -a | grep vm.swappiness
vm.swappiness = 30
sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
sudo sysctl -p 
vm.swappiness = 1
