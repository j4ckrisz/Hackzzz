---
description: >-
  https://portswigger.net/web-security/file-upload/lab-file-upload-web-shell-upload-via-content-type-restriction-bypass
---

# Web shell upload via Content-Type restriction bypass

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/Web_shell_upload_via_Content_Type_restriction_bypass.png" alt=""><figcaption></figcaption></figure>

* This time its haves a file upload restriction, and is the same objective as the first challenge
* We need to get the file content of **/home/carlos/secret.**

<figure><img src="../../../../../.gitbook/assets/Web_shell_upload_via_Content_Type_restriction_bypass1.png" alt=""><figcaption></figcaption></figure>

* If you try to upload the malicious file of the previous challenge, will not work
* How you can bypass this? well, if you change the file extension on your machine, you change the **Content-Type** of the requests and bypass the restriction as you can see in the following image.

<figure><img src="../../../../../.gitbook/assets/Web_shell_upload_via_Content_Type_restriction_bypass2.png" alt=""><figcaption></figcaption></figure>
