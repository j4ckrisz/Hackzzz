---
description: >-
  https://portswigger.net/web-security/sql-injection/examining-the-database/lab-querying-database-version-mysql-microsoft
---

# SQL injection attack, querying the database type and version on MySQL and Microsoft

**Level:** <mark style="color:blue;">**Practitioner**</mark>

<figure><img src="../../../../../.gitbook/assets/SQLinjectionattackqueryingthedatabasetypeandversiononMySQLandMicrosoft1 (1).png" alt=""><figcaption></figcaption></figure>

* To get the version of the **MySQL** database we just need to change a single space when we enumerate the columns with _**NULL**_ spaces.

<figure><img src="../../../../../.gitbook/assets/SQLinjectionattackqueryingthedatabasetypeandversiononMySQLandMicrosoft2.png" alt=""><figcaption></figcaption></figure>

* In one of the following _**NULL**_ spaces replace it with _**@@version**_**.**
