## Useful Codes

### NFS Setup

For installation of nfs-utils, setting and starting NFS server

```
sudo yum install -y nfs-utils
sudo systemctl enable nfs-server
sudo systemctl start nfs-server
```

Remember to modify /etc/exports to allow for access.

###Firewall

Adds to firewall NFS service, can also disable (during testing/non prod env)

```
sudo firewall-cmd --add-service=nfs --permanent
sudo firewall-cmd --reload
```

```
sudo systemctl stop firewalld
sudo systemctl start firewalld
sudo systemctl status firewalld
```

Installation of Java

```
sudo yum install -y java-11-openjdk
```
