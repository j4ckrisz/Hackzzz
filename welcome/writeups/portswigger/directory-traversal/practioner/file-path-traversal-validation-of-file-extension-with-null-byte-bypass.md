---
description: >-
  https://portswigger.net/web-security/file-path-traversal/lab-validate-file-extension-null-byte-bypass
---

# File path traversal, validation of file extension with null byte bypass

**Level:** <mark style="color:blue;">**Practitioner**</mark>

<figure><img src="../../../../../.gitbook/assets/Filepathtraversalvalidationoffileextensionwithnullbytebypass1.png" alt=""><figcaption></figcaption></figure>

* In the following challenge if we don't do something we will never get the file.

<figure><img src="../../../../../.gitbook/assets/Filepathtraversalvalidationoffileextensionwithnullbytebypass2.png" alt=""><figcaption></figcaption></figure>

* This time we used the simple `../../../etc/passwd`.
* Now we need to bypass the file extension somehow, use a null char **%00** followed by .png .
