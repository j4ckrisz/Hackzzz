---
description: >-
  https://portswigger.net/web-security/access-control/lab-user-id-controlled-by-request-parameter-with-data-leakage-in-redirect
---

# User ID controlled by request parameter with data leakage in redirect

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/Useridcontroledbyrequestparameterwithdataleakageinredirect1.png" alt=""><figcaption></figcaption></figure>

* In this lab we continue playing with the id parameter on my account page
* Start making some recon with Burp Suite and found this.

<figure><img src="../../../../../.gitbook/assets/Useridcontroledbyrequestparameterwithdataleakageinredirect3.png" alt=""><figcaption></figcaption></figure>

* **302 status code** from the server, basically in this case is for **redirecting** us to another page, that is `/login.`
* Take a look at the response of the **302-server response**, you will see that is letting us to see the user's password.&#x20;

<figure><img src="../../../../../.gitbook/assets/Useridcontroledbyrequestparameterwithdataleakageinredirect2.png" alt=""><figcaption></figcaption></figure>

* There is the **API Key** **from the user Carlos.**
* Remember Do your homework by making recon on the features, functions, parameters and stuff on the page.
