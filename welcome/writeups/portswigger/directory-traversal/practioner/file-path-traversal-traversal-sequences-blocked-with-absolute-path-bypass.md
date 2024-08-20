---
description: >-
  https://portswigger.net/web-security/file-path-traversal/lab-absolute-path-bypass
---

# File path traversal, traversal sequences blocked with absolute path bypass

**Level:** <mark style="color:blue;">**Practitioner**</mark>

<figure><img src="../../../../../.gitbook/assets/Filepathtraversaltraversalsequencesblockedwithabsolutepathbypass (1).png" alt=""><figcaption></figcaption></figure>

* In this challenge, just the sequences like `../../../../` or other are blocked.

<figure><img src="../../../../../.gitbook/assets/dirpathtraversal_blocked2.png" alt=""><figcaption></figcaption></figure>

* Try with just passing **"from the root path, open passwd"**
* Just use **/** and if its not blocked, problem solved.
