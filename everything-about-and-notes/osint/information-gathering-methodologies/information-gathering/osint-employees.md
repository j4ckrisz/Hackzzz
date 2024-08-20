---
description: Making reconnaisannce to employees in the company
---

# OSINT Employee's

## OSINT

### Wikipedia

* While we typically won’t find email addresses on a company’s Wikipedia page, we can find other helpful information such as number of employees and names of high-ranking employees (C-Level employees, board members, etc).
* Another bit of information we look for on Wikipedia are recent awards or recognition.

### Hunter.io

* Compiles email addresses from open-source intelligence gathering and makes them searchable by domain.

### LinkedInt

* To begin employee enumeration through LinkedIn, we start with the tool [LinkedInt](https://github.com/vysecurity/LinkedInt).&#x20;
* LinkedInt uses a combination of LinkedIn API calls and Hunter.io searches to find the correct company.
* The tool then finds LinkedIn profiles registered with the domain you originally searched for and generates an HTML page with profile picture, name, email address, and job title.

### Peasant

* **Peasant** has a lot of the same functionality of **LinkedInt** but also provides functionality to blanket a company with connection requests and spoof your profile to look like another.

### Public Breach Data

* Attackers will often sell or distribute email and password combinations once a website or company has been breached.
* Eventually, the data ends up on torrent sites, forums, and sites like HaveIBeenPwned, Dehashed, and Pastebin.
