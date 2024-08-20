---
description: >-
  https://portswigger.net/web-security/sql-injection/examining-the-database/lab-listing-database-contents-non-oracle
---

# SQL injection attack, listing the database contents on non-Oracle databases

**Level:** <mark style="color:blue;">**Practitioner**</mark>

<figure><img src="../../../../../.gitbook/assets/SQLinjectioattacklistingheatabaseontentsnon-Oracledatabases1 (1).png" alt=""><figcaption></figcaption></figure>

* Same as the other challenges, nothing new, just we need to get some **DB's info**.
* As always enumerate the columns
* In this example I'm using _**NULL**_ spaces to get the number of columns.

<figure><img src="../../../../../.gitbook/assets/SQLinjectioattacklistingheatabaseontentsnon-Oracledatabases2 (3).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../../../.gitbook/assets/SQLinjectioattacklistingheatabaseontentsnon-Oracledatabases3 (1).png" alt=""><figcaption></figcaption></figure>

* Use the public database and get their respective names.
