---
description: >-
  https://portswigger.net/web-security/file-upload/lab-file-upload-remote-code-execution-via-web-shell-upload
---

# Remote code execution via web shell upload

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/Remote_code _execution_via_web_shell_upload.png" alt=""><figcaption></figcaption></figure>

* Here in this lab is a simple demonstration of a file upload vulnerability.
* We need to access a file in **/home/carlos/secret**.

<figure><img src="../../../../../.gitbook/assets/Remote_code _execution_via_web_shell_upload1.png" alt=""><figcaption></figcaption></figure>

* Try to upload just a single malicious file like is show in the image.
* We see that we can upload **php** file without any restriction.

<figure><img src="../../../../../.gitbook/assets/Remote_code _execution_via_web_shell_upload2.png" alt=""><figcaption></figcaption></figure>

* Now to see the content of **/home/carlos/secret**, use **get\_file\_contents()** php function.
* Once uploaded, set the URL and you will see the flag to submit.
