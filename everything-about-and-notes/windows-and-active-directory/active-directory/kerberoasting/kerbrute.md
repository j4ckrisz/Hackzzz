# Kerbrute

<figure><img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse1.mm.bing.net%2Fth%3Fid%3DOIP.bOAgn8VhjjhKKLataKTe7QHaDt%26pid%3DApi&#x26;f=1&#x26;ipt=581b3b5cf03f598fc20fe65cf899457e2d8453ff75f26ad1576dfe460f2b923f&#x26;ipo=images" alt=""><figcaption></figcaption></figure>

## Kerbrute Enumeration

**Kerbrute** is a popular enumeration tool used to **brute force** and **enumerate** valid active directory users by **abusing Kerberos pre-authentication**.

**Kerbrute Binary:**

* [https://github.com/ropnop/kerbrute/releases](https://github.com/ropnop/kerbrute/releases)

### userenum

```java
./kerbrute userenum --dc <domain.local> -d <domain> <path-to-user-wordlist>
```

### bruteuser

```java
./kerbrute bruteuser --dc <domain-ip> --domain <domain> rockyou.txt sqlservice
```
