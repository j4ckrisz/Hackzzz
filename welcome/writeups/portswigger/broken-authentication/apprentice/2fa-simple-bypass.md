---
description: >-
  https://portswigger.net/web-security/authentication/multi-factor/lab-2fa-simple-bypass
---

# 2FA simple bypass

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/2fabypass1.png" alt=""><figcaption></figcaption></figure>

* This is just a simple 2FA Bypass, that it.
* First, start authenticating to see what we can do with it.

<figure><img src="../../../../../.gitbook/assets/2fabypass2.png" alt=""><figcaption></figcaption></figure>

* Okay once we put the password and username, it tells us that an email has been sent to the respective user email.

<figure><img src="../../../../../.gitbook/assets/2fabypass3.png" alt=""><figcaption></figcaption></figure>

* Just to see what I can modify I put the 4-digit pin into it.
* Nothing interesting for now.

<figure><img src="../../../../../.gitbook/assets/2fabypass4.png" alt=""><figcaption></figcaption></figure>

* Knowing that is a _**simple 2FA Bypass**_, I've seen that once you log in with the user credentials there is a `/login2`
* So, try to change it to `/my-account` or `/login1` to see what can happen.

<figure><img src="../../../../../.gitbook/assets/2fabypass5.png" alt=""><figcaption></figcaption></figure>

* Just getting out the `/login2` you get into the user account, that's how simple it is.

<figure><img src="../../../../../.gitbook/assets/2fabypass6.png" alt=""><figcaption><p>work done</p></figcaption></figure>
