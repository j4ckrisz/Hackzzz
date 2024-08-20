# AD Enumeration

## Port scanning

* nmap -A -p- -T3 --open -vvv -Pn **\<IP> -oN \<output\_file>**
* Important ports are **88, 445** and **139**.

## SMB Enumeration

{% tabs %}
{% tab title="smbclient" %}
smbclient //\<IP>/interesting-directory -c 'recursive ; ls' **- Fast smb directory enumeration**
{% endtab %}

{% tab title="smbmap" %}
smbmap -H \<IP> -U ''"
{% endtab %}
{% endtabs %}

## RPC Enumeration

{% tabs %}
{% tab title="Authenticating" %}
rpcclient -U '' -N \<IP> **- Without password**

rpcclient -U '' -P '' \<IP> **- Using a password**
{% endtab %}

{% tab title="Enumerating RPC" %}
enumdomusers - **Enumerate all domain users**

querygroupmem 0x200 - **Enumerate all the admin users of the domain.**

queryuser 0x1f4 - **Enumerate user information using the rid.**
{% endtab %}
{% endtabs %}

## LDAP Enumeration

### Using ldapsearch and ldapdomaindump

{% tabs %}
{% tab title="ldapsearch" %}
ldapsearch -H ldap://\<IP> -x -s base namingcontext

ldapsearch -H ldap://\<IP> -x -s -b 'DC=tld,DC=local' '(objectClass=User)' 'sAMAccountName' | grep sAMAccountname
{% endtab %}

{% tab title="ldapdomaindump" %}
ldapdomaindump.py -u 'domain.local\user' -p 'password123' \<IP>
{% endtab %}
{% endtabs %}

## Kerberos

{% tabs %}
{% tab title="User enumeration" %}
kerbrute userenum --dc \<domain.local> -d \<domain> \<path-to-user-wordlist>
{% endtab %}

{% tab title="Brute-Forcing Users" %}
kerbrute bruteuser --dc \<domain-ip> --domain \<domain> rockyou.txt sqlservice
{% endtab %}
{% endtabs %}

### Kerberoasting

{% content-ref url="kerberoasting/" %}
[kerberoasting](kerberoasting/)
{% endcontent-ref %}

## Crackmapexec



{% tabs %}
{% tab title="Brute-Force" %}
crackmapexec smb targets.txt -u users.txt -p passwords.txt

crackmapexec smb targets.txt -u users.txt -p passwords.txt --continue-on-success
{% endtab %}

{% tab title="Get Domain Password Policy" %}
crackmapexec smb 192.168.1.0/24 -u username -p 'password' **--pass-pol**&#x20;
{% endtab %}

{% tab title="Password / Username Spraying" %}
crackmapexec smb 192.168.1.0/24 -u userfile -p passwordfile --no-bruteforce
{% endtab %}

{% tab title="Scan for vulnerabilities" %}
`crackmapexec smb <ip> -u '' -p '' -M zerologo` _**- Zerologon**_

`crackmapexec smb <ip> -u '' -p '' -M petitpotam` _**- petitpotam**_

`crackmapexec smb <ip> -u 'user' -p 'pass' -M nopac` _**- NoPac** >> You need credentials dor this one._
{% endtab %}
{% endtabs %}

{% embed url="https://wiki.porchetta.industries/" %}

## Evil-Winrm

{% tabs %}
{% tab title="Connecting through winrm" %}
evil-winrm -i \<IP> -u 'user' -p 'password'
{% endtab %}
{% endtabs %}
