---
description: >-
  https://portswigger.net/web-security/file-path-traversal/lab-superfluous-url-decode
---

# File path traversal, traversal sequences stripped with superfluous URL-decode

**Level:** <mark style="color:blue;">**Practitioner**</mark>

<figure><img src="../../../../../.gitbook/assets/FilepathtraversaltraversalsequencesstrippedwithsuperfluousURL-decode1 (1).png" alt=""><figcaption></figcaption></figure>

* This challenge is simple, just URL encode `../../../etc/passwd`.

<figure><img src="../../../../../.gitbook/assets/FilepathtraversaltraversalsequencesstrippedwithsuperfluousURL-decode2.png" alt=""><figcaption></figcaption></figure>

* The server does not interpretate the URL encode so that's why we are able to bypass this.
