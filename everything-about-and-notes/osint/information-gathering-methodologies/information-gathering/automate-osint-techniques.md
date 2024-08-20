# Automate OSINT techniques

### The Harvester

* This tool gathers subdomain names, IP addresses, email addresses and employee names while only needing an initial domain name to start.
* In order to use this tool you will need the following API Keys: _Bing, Github, Hunter.io, Intelx, SecurityTrails, Shodan, Spyse._
* **theHarvester** will work fine without these API keys but the search results may be limited.

{% code title="Running theHarvester" overflow="wrap" %}
```bash
python3 theHarvester.py -d <target_domain> -b all
```
{% endcode %}

### Amass

* Amass does not perform OSINT on employee names or email, it makes up for it in the large amount of subdomain OSINT sources.
* Amass is set up as a suite of tools that can search for subdomains, ASNs, and IP addresses as well as perform brute force subdomain discovery.

{% code title="Amass different scan one-liners." %}
```bash
 # Search for domain names associated with target domain through reverse whois:
 amass intel -d <target_domain> -whois
 
 # Search for company name is ASN names:
 amass intel -org <target_organization>
 
 # Search for domain names, associated IP addresses in an ASN, and prints where Amass found them:
 amass intel -asn <target_asn> -ip -src
 
 # Search for subdomains found strictly in open-source intelligence resources:
 amass enum -d <target_domain> -passive
 
 # Search for subdomains and verify info about the host through direct connections:
 amass enum -d <target_domain> -active
 
 # Brute force subdomains using a mask of aaa-[a-z][a-z][a-z]:
 amass enum -d <target_domain> -active -brute -wm "aaa-?l?l?l" 
```
{% endcode %}

### Recon-ng

* Recon-NG is more of a framework of tools rather than just one tool.
* What makes it great is the extensibility through the Recon-NG Marketplace.
* You can choose which addons you want to install as well as create your own for others to use.

{% embed url="https://www.youtube.com/watch?list=PLBf0hzazHTGOg9taK90uFjdcb8UgGfRKZ&v=1RCqOhb0yxE" %}
