# SSH

### Forward RDP from internal host to Attacking Machine on port 1337.

```java
ssh -L <LocalHost>:<Port>:<IP-To-Forward-From>:<Port> <User>@<IP>
ssh -L 127.0.0.1:1337:10.200.48.150:3389 root@10.200.48.200 -i id_rsa
```

### Forward remote port 80 to local port 80.

```java
ssh atena@10.10.72.69 -L 80:127.0.0.1:80
ssh <User>@<IP> -L <Local-Port>127.0.0.1<Remote-Port>
```

### Dynamic SSH Port Forwarding

```java
ssh -i <id_rsa> <User>@<IP> -D <Proxychains-Port>
ssh -i id_rsa errorcauser@10.10.254.201 -D 1080
```
