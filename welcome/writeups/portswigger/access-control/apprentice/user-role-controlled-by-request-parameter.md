---
description: >-
  https://portswigger.net/web-security/access-control/lab-user-role-controlled-by-request-parameter
---

# User role controlled by request parameter

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/User_role_controlled_by_request_parameter.png" alt=""><figcaption></figcaption></figure>

* Now we need to get in some way into administrative panel but this time we will be exploiting a forgeable cookie.

<figure><img src="../../../../../.gitbook/assets/access_controluser_role2.png" alt=""><figcaption><p>admin directory</p></figcaption></figure>

* Looking at the **/admin** directory and my **cookies**, we see that there is a cookie called Admin, and it has the value of **False.**
* What happens if we change the admin cookie to true and try to access admins directory.

<figure><img src="../../../../../.gitbook/assets/access_controluser_role3.png" alt=""><figcaption></figcaption></figure>

Voila! we magically access the **/admin** directory and delete user Carlos.
