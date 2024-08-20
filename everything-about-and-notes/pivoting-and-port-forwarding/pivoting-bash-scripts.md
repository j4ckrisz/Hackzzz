# Pivoting Bash Scripts

### Host discovery Script

```bash
#!/bin/bash

host=("10.200.87") # change this

for host in ${host[@]}; do


        echo -e "\n[+] Enumerating $host.0/24"

        for i in $(seq 1 254);do

                timeout 1 bash -c "ping -c 1 $host.$i" &> /dev/null && echo "[+] Host $host.$i - ACTIVE" &

        done; wait

done
```

### Port Scanner Script

```bash
#!/bin/bash

host=("<host-to-scan>")

for host in ${host[@]}; do

        echo -e "\n[+] Scanning Ports: $host"

        for i in $(seq 1 10000);do

                timeout 1 bash -c "echo '' > /dev/tcp/$host/$i" 2> /dev/null && echo "[+] Port $i - ACTIVE" &


        done; wait

done
```
