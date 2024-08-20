# GPP cPassword Attack

## What is GPP?

* Group policies preferences allowed admins to create policies using embedded credentials.
* These credentials were encrypted and placed in a **"cPassword"**

### Why is vulnerable?

* The key was **accidentally released by Microsoft**
* Patched in **MS14-025** but doesn't prevent previous uses.
* The key was stored in **SYSVOL**
* **Any Domain User can read the policy**

### Resources

* [https://www.rapid7.com/blog/post/2016/07/27/pentesting-in-the-real-world-group-policy-pwnage/](https://www.rapid7.com/blog/post/2016/07/27/pentesting-in-the-real-world-group-policy-pwnage/)

