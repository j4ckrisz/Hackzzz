---
description: https://portswigger.net/web-security/information-disclosure
---

# 📑 Information Disclosure

## Intro

**Information disclosure**, also known as information leakage, is when a website unintentionally **reveals sensitive information to its users.**&#x20;

Depending on the context, websites may **leak all kinds of information to a potential attacker like:**

* Data about other users, such as usernames or financial information
* Sensitive commercial or business data
* Technical details about the website and its infrastructure

### Information Disclosure Examples

* Revealing the names of **hidden directories**, their structure, and their contents via a `robots.txt` file or directory listing
* Providing access to source code files via temporary backups
* Explicitly mentioning database table or column names in error messages
* Unnecessarily exposing highly sensitive information, such as credit card details
