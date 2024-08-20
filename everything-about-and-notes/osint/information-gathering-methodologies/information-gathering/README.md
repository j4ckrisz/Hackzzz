---
description: Gathering information about a Company/Website
---

# Information Gathering

## Website Info

**Wikipedia** - Entries on Wikipedia will often have a biography of the company including associated domains and can also contain histories of mergers, acquisitions, and subsidiary companies. Using this list of affiliated companies, an attacker can potentially find additional domains associated with the target. In the case of the selected company, Wikipedia indicates a history of acquisitions.

**DNSdumpster** - This site provides a wealth of information about a target domain such as MX records, TXT records, ASN identification, and a list of subdomains.

**Whois** - is a query and response protocol that is used for querying databases that store an Internet resource's registered users or assignees.

### Emails Associated

**Hunter.io** - Is a tool for finding professional email addresses, usually for outreach. This is one of the more accurate email finder tools.

**Intelx(phonebook)** - This is the email hunter of intelx.

### **Hurricane** **Electric BGP Toolkit**

* Using the data found with **DNSDumpster**, we can continue host and IP address discovery by searching the [Hurricane Electric BGP Toolkit](https://bgp.he.net/) for company name, IP address/CIDR range, and ASNs.
* Searching for the company name will return a list of ASNs and CIDR IP address ranges. While not all of the results will be relevant to our target, additional ASNs can be found in the results.

### Shodan

* **Shodan** is a search engine for devices on the internet. When a device is found, they record details about the available services, headers returned during interactions, and geolocation of the physical host. We can use this information when profiling the attack surface of our target.

### **SSL Certificate Search**

* Provide results based on **SSL certificates** observed while scanning the internet. We use the domains shown in the results from both to help find additional hosts.

### **SpyOnWeb**

* Tool for finding alternate domains for an IP address or URL. **SpyOnWeb** accepts IP addresses or URLs and returns information about what is hosted.

### **Archive.org**

* The WayBack Machine, _is constantly archiving websites and making them searchable_.\
  Once we find a backup of a website, we use the tool [Wayback Machine\
  Downloader](https://github.com/hartator/wayback-machine-downloader) to pull an offline copy.

### **Google Dorking**

* Use some google dorks to search for some confidential exposed files like pdf, xlsx, txt, etc.

**Try to gain the most useful information.**

### Job Listings

* A good way to find which software and security suites a company employs is to search through job postings.
* We look for keywords such as **‘IT’**, **‘helpdesk’**, **‘cybersecurity analyst’,** ‘**developer’**, or ‘**programmer’**. Job postings often contain software suites, frameworks, and security platforms as requirements for the applican

## Use the Gathered Info to build a strategy

* Based on the information you gather build a plan to the admin users or users to give you the initial foothold on the surface.
* **Example**: _Send an email with a malicious content and pretend to be from the company that they are hosting their website._

_Credits to:_

{% embed url="https://redsiege.com/tools-techniques/" %}
