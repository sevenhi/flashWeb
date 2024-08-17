# openwrt

- dnsmasq

```bash
vi /etc/dnsmasq.conf

# add following lines
dhcp-option=tag:proxy,3,192.168.2.2                   # set tag with dns
dhcp-option=tag:proxy,6,192.168.2.2                   # set tag with router
dhcp-host=E0:D4:E8:F2:41:DA,set:proxy,192.168.2.166   # link device to tag

# restart dns
/etc/init.d/dnsmasq restart
```

- AdguardHome

```bash
# dns provider
61.132.163.68
202.102.213.68
114.114.114.114
```