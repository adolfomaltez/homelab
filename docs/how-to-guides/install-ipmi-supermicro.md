# Configure LACP on Juniper EX-2200

```ssh
root@juniper-01> configure
edit
set interfaces ge-0/0/36 ether-options 802.3ad ae0
set interfaces ge-0/0/37 ether-options 802.3ad ae0
set interfaces ae0 aggregated-ether-options lacp active
set interfaces ae0 aggregated-ether-options lacp periodic slow
set interfaces ae0 unit 0 family ethernet-switching port-mode trunk native-vlan-id 11
```


# References:

- https://ahelpme.com/linux/tips/configure-and-mount-samba-share-in-supermicro-ipmi-virtual-media-cd-rom/
