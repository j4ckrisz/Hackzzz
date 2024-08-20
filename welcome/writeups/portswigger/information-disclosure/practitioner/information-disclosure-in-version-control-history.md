---
description: >-
  https://portswigger.net/web-security/information-disclosure/exploiting/lab-infoleak-in-version-control-history
---

# Information disclosure in version control history

**Level:** <mark style="color:blue;">**Practitioner**</mark>

<figure><img src="../../../../../.gitbook/assets/intro_dic_p.png" alt=""><figcaption></figcaption></figure>

* Practitioner level, we need to get the admin password this time.

<figure><img src="../../../../../.gitbook/assets/Info_disc_p1.png" alt=""><figcaption></figcaption></figure>

* To automate a little recon, I used _**dirsearch**_ and found a **/.git** exposed.
* So, let's make recursive **wget** on the directory and make some git recon.

<figure><img src="../../../../../.gitbook/assets/info_disc_p2.png" alt=""><figcaption></figcaption></figure>

* Now in the image below I enumerate the git a little bit and one of the commits contains the admin password.
* Just Login with the credentials and delete the user, Carlos.&#x20;

<figure><img src="../../../../../.gitbook/assets/info_disc_pn3.png" alt=""><figcaption></figcaption></figure>
