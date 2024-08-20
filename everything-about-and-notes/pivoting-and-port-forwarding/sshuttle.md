# sshuttle

```java
sshuttle -r root@10.200.87.200 --ssh-cmd "ssh -i <id_rsa>" <CIDR>/24 -x <machine-ip>

// Examples:
sshuttle -r user@address --ssh-cmd "ssh -i KEYFILE" SUBNET
sshuttle -r user@172.16.0.5 172.16.0.0/24 -x 172.16.0.5
sshuttle -r user@172.16.0.5 --ssh-cmd "ssh -i private_key" 172.16.0.0/24
sshuttle -r root@10.200.87.200 --ssh-cmd "ssh -i id_rsa_root" 10.200.87.0/24 -x 10.200.87.200
```
