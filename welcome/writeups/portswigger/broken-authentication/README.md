---
description: https://portswigger.net/web-security/authentication
---

# 🧃 Broken Authentication

## What is authentication?

Authentication is the **process of verifying the identity of a given user or client.** In other words, it involves making sure that they really are who they claim to be.

There are three authentication factors into which different types of authentications can be categorized:

* Something you **Know.** Ex: **Security Question**
* Something you **Have.** Ex: **a physical object like a mobile phone or security token**
* Something you **are or do.** Ex: **Your biometrics or patterns of behavior.**

### How do authentication vulnerabilities arise? <a href="#how-do-authentication-vulnerabilities-arise" id="how-do-authentication-vulnerabilities-arise"></a>

* The authentication **mechanisms are weak** because they fail to adequately protect against brute-force attacks.
* Logic flaws or poor coding in the implementation allow the authentication mechanisms to be bypassed entirely by an attacker. This is sometimes referred to as **"broken authentication".**
