
[root@nodo1 cloudera]# cat /etc/krb5.conf
# Configuration snippets may be placed in this directo                                                                                                                  ry as well
includedir /etc/krb5.conf.d/

[logging]
 default = FILE:/var/log/krb5libs.log
 kdc = FILE:/var/log/krb5kdc.log
 admin_server = FILE:/var/log/kadmind.log

[libdefaults]
 default_realm = GUSTAVOACO.HQ
 dns_lookup_realm = false
 dns_lookup_kdc = false
 ticket_lifetime = 24h
 renew_lifetime = 7d
 forwardable = true
 udp_preference_limit = 1
 default_tgs_enctypes = arcfour-hmac
 default_tkt_enctypes = arcfour-hmac

[realms]
  GUSTAVOACO.HQ = {
  kdc = nodo2.gus.com
  admin_server = nodo2.gus.com
 }

[domain_realm]
   .gus.com = GUSTAVOACO.HQ
   gus.com = GUSTAVOACO.HQ
