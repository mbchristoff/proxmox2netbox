proxmox2netbox
==============

This script export proxmox VM information in CSV format to be importable by
Netbox.

Example:

```
$ ./proxmox2netbox --host 12.23.34.45:8006 --username $username --password $password  --cluster $cluster
name,cluster,status,vcpus,memory,disk,comments
my-vm,my-cluster,Active,4,8192,50,type=qemu vmid=100 node=pve1
...
```

Note
----

This script is just a fork from https://github.com/mrproper/proxmox-ve-api-perl/blob/master/examples/list_qemus.pl
