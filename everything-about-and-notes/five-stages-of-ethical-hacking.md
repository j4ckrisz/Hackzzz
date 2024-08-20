---
cover: >-
  https://images.unsplash.com/photo-1562860149-691401a306f8?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHw5fHxoYWNrZXJ8ZW58MHx8fHwxNjg4MDA5MjQ2fDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# 🥷 Five stages of Ethical Hacking

## Hacking Methodology

<table data-view="cards"><thead><tr><th></th><th></th><th></th></tr></thead><tbody><tr><td></td><td><strong>Reconnaissance ---></strong></td><td></td></tr><tr><td></td><td><strong>Scanning &#x26; Enumeration</strong></td><td>---></td></tr><tr><td></td><td><strong>Gaining Access &#x26; Explotation</strong> ---></td><td></td></tr><tr><td></td><td><strong>Maintaining Access ---></strong></td><td></td></tr><tr><td></td><td><strong>Covering Tracks</strong> </td><td></td></tr></tbody></table>

## Reconnaissance

There are 2 types of Reconnaissance:

* **Active and Passive**

**Passive**: All info available on the internet using **Google, LinkedIn, Facebook, Twitter, etc**.

**Active**:  This type of recon is when we use tools like **Nmap, Nessus, Nikto.**

## Scanning & Enumeration

In this phase we take a look using **active recon**. Looking for **open ports**, **vulnerabilities**, and different items. What returns on these results when we do the **scanning**, we also perform what is called **enumeration**. Example:

* Knowing the version of the **webserver** like **Apache 1.x**, then we look into google to see if is vulnerable.

## Gaining Access & Exploitation

This is when we **exploit** a **vulnerability** to try to gain access to the **network**, once we do this, the process tend to repeat. Example:

* You see that the **SMB** Protoco**l** is **Vulnerable** to **EternalBlue** and you continue to exploit. You finally **get access** to that computer/machine.

## Maintaining Access

This is for in case we get **kicked out** or a **user shuts down their computer**, **how do we maintain that access**, so when they turn their computer back on, we still have access to it.

## Covering Tracks

You want to **delete** any kind of **log** or **malware** which is more **important as a pen tester.**  Any **accounts that you create for any reason.**  In **resume** this is more a **Clean Up.**

