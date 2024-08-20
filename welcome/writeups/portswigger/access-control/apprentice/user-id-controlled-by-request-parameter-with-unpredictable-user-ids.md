---
description: >-
  https://portswigger.net/web-security/access-control/lab-user-id-controlled-by-request-parameter-with-unpredictable-user-ids
---

# User ID controlled by request parameter, with unpredictable user IDs

**Level:** <mark style="color:green;">**Apprentice**</mark>

<figure><img src="../../../../../.gitbook/assets/User_ID_controlled_by_request_parameter_with_unpredictable_user_IDs (2).png" alt=""><figcaption></figcaption></figure>

* In this lab we need to get access to the API Key of Carlos again.
* If you try to get access to another user account by changing the id parameter to Carlos, we will not see anything interesting
* Now the users have an identifier random number.

<figure><img src="../../../../../.gitbook/assets/user_unpre2.png" alt=""><figcaption></figcaption></figure>

* Making some recon on the posts in the page, you will see that you can see another user id random number by clicking on a posts of the respective user

<figure><img src="../../../../../.gitbook/assets/user_unpre3.png" alt=""><figcaption></figcaption></figure>

* Try to copy the `userid` from one of the posts from user Carlos.
* Paste the user id from the post into your `my-account` userid and you will that we're log into the account of carlos to complete the lab.

<figure><img src="../../../../../.gitbook/assets/user_unpre4.png" alt=""><figcaption></figcaption></figure>
