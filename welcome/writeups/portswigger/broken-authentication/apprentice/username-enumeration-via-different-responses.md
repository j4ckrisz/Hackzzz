---
description: >-
  https://portswigger.net/web-security/authentication/password-based/lab-username-enumeration-via-different-responses
---

# Username enumeration via different responses

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/userenum_auth_1.png" alt=""><figcaption></figcaption></figure>

* The lab provided here has a potential way to _**enumerate users**_ on the `my-account` form.
* I will be playing this time with **Burp Suite** to make it "faster" and easy.
* Download the 2 wordlists presented on the page

<figure><img src="../../../../../.gitbook/assets/userenum_auth_2.png" alt=""><figcaption><p>Burp Suite User Enumeration</p></figcaption></figure>

* Let's use the intruder for this, to make a _**sniper attack**_ and use a **simple list** to enumerate the users first.
* As you see in the burp suite example, I filter by the length of the response.
* Later that, I search for the keyword `Invalid username.`
* Same process to know the password

<figure><img src="../../../../../.gitbook/assets/userenum_auth3.png" alt=""><figcaption></figcaption></figure>

* Once you get credentials login as the valid user and its respective password.
