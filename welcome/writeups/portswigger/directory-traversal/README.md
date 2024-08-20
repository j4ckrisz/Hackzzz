---
description: https://portswigger.net/web-security/file-path-traversal
---

# 🪜 Directory Traversal

## What is Directory Traversal?

* Is a web security vulnerability that allows an attacker to _**read arbitrary files**_ and also might be able to _**write to arbitrary** files_ on the server that is running an application.

### What might include:

* Application Code and Data
* Credentials for back-end systems
* Sensitive operating system files

### Quick Example:

* The application implements no defenses against directory traversal attacks, so an attacker can request the following URL **to retrieve an arbitrary file from the server's filesystem:**

```
https://insecure-website.com/loadImage?filename=../../../etc/passwd
```

### Top 25 parameters

Look for this vulnerability, in these parameters.

```
?cat={payload}
?dir={payload}
?action={payload}
?board={payload}
?date={payload}
?detail={payload}
?file={payload}
?download={payload}
?path={payload}
?folder={payload}
?prefix={payload}
?include={payload}
?page={payload}
?inc={payload}
?locate={payload}
?show={payload}
?doc={payload}
?site={payload}
?type={payload}
?view={payload}
?content={payload}
?document={payload}
?layout={payload}
?mod={payload}
?conf={payload}
```
