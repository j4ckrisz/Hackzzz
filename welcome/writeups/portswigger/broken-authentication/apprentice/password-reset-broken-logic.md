---
description: >-
  https://portswigger.net/web-security/authentication/other-mechanisms/lab-password-reset-broken-logic
---

# Password reset broken logic

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/Password_reset_logic1.png" alt=""><figcaption></figcaption></figure>

* The following lab basically says Reset another's user password.
* So, go straight to it.

<figure><img src="../../../../../.gitbook/assets/Password_reset_logic2.png.png" alt=""><figcaption></figcaption></figure>

* Click on the Forgot Password

<figure><img src="../../../../../.gitbook/assets/Password_reset_logic3.png" alt=""><figcaption></figcaption></figure>

* I made the common process of resetting the password for my account
* Start to intercept literally every request to make some recon.

<figure><img src="../../../../../.gitbook/assets/Password_reset_logic4.png" alt=""><figcaption></figcaption></figure>

* Finally, I get Something Interesting in the parameters and info we are passing once we put our new password.

<figure><img src="../../../../../.gitbook/assets/Password_reset_logic5.png" alt=""><figcaption></figcaption></figure>

* There is a username parameter that if we change it to user Carlos, we can change his password using my respective new password form.

<figure><img src="../../../../../.gitbook/assets/Password_reset_logic6.png" alt=""><figcaption></figcaption></figure>
