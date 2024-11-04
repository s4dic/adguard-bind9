# adguard-bind9
Create your own adguard &amp; bind9 on the same docker compose

# adguard-setup
On your server, fix ip and then remove dhclient & reboot:
```apt remove isc-dhcp-client -y```
```reboot```

Setup your adguard here http://YOURIP:8830/ just press next and setup an account (don't change anything else)

IMPORTANT:
In Adguard pannel go to "settings" and "DNS settings"
In "Upstream DNS servers" AND "Bootstrap DNS servers" add this IP: "172.30.0.3", press "test upstreams" and "Apply"

You DNS is now functional, don't forget, your adguard port now is 80 (http://YOURIP:80/)
