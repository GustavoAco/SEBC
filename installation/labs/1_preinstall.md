<h3>Cambiando Swappines</h3>
<code>sysctl -a | grep vm.swappiness
<br>vm.swappiness = 30
sudo sysctl -w vm.swappiness=1
vm.swappiness = 1
sudo sysctl -p 
vm.swappiness = 1
</code>

<h3>Formateando Discos y montandolos </h3>
<code>
mkfs.xfs -f /dev/sdd
mkfs.xfs -f /dev/sdc
</code>
<br>
<code>
mount -t xfs /dev/sdd /media/hhd1/
mount -t xfs /dev/sdd /media/hhd2/
 </code>

<h3> Pruebas DNS </h3>
<code>
nslookup node1.gus.com
Server:         10.0.0.110
Address:        10.0.0.110#53

Name:   node1.gus.com
Address: 10.0.0.110
</code>
<br>
<h3>Dig</h3>
<code>
dig -x 10.0.0.110

; <<>> DiG 9.9.4-RedHat-9.9.4-51.el7 <<>> -x 10.0.0.110
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 43228
;; flags: qr aa rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
;; QUESTION SECTION:
;110.0.0.10.in-addr.arpa.       IN      PTR

;; ANSWER SECTION:
110.0.0.10.in-addr.arpa. 0      IN      PTR     node1.gus.com.

;; Query time: 0 msec
;; SERVER: 10.0.0.110#53(10.0.0.110)
;; WHEN: Fri Dec 01 03:20:02 UTC 2017
;; MSG SIZE  rcvd: 79
</code>
<h3>Servicios a detener <strong>Firewalld ,chronyd ,selinux y tuned</strong></h3>
<code>
 sestatus
SELinux status:                 disabled
sestatus
SELinux status:                 disabled
 
 
systemctl stop firewalld.service
systemctl disable firewalld.service

systemctl stop chronyd.service
systemctl disable chronyd.service

systemctl stop tuned.service
systemctl disable tuned.service

</code>


