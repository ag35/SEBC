```
[logging]
 default = FILE:/var/log/krb5libs.log
 kdc = FILE:/var/log/krb5kdc.log
 admin_server = FILE:/var/log/kadmind.log

[libdefaults]
 default_realm = AG35.IL
 dns_lookup_realm = false
 dns_lookup_kdc = false
 ticket_lifetime = 24h
 renew_lifetime = 7d
 forwardable = true
 udp_preference_limit = 1
 default_tgs_enctypes = arcfour-hmac
 default_tkt_enctypes = arcfour-hmac 

[realms] 
  AG35.IL = {
  kdc = ip-172-31-56-113.ec2.internal 
  admin_server = ip-172-31-56-113.ec2.internal 
 }

[domain_realm]
   .ec2.ineternal = AG35.IL
   ec2.ineternal = AG35.IL

```