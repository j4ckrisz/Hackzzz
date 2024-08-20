---
description: >-
  https://portswigger.net/web-security/sql-injection/union-attacks/lab-find-column-containing-text
---

# SQL injection UNION attack, finding a column containing text

**Level:** <mark style="color:blue;">**Practitioner**</mark>

<figure><img src="../../../../../.gitbook/assets/SQL_injection_UNION_attack_finding_a_column_containing_text1.png" alt=""><figcaption></figcaption></figure>

* This time what we need to do is find a writable field to retrieve info about other tables, users, DB's.

<figure><img src="../../../../../.gitbook/assets/SQL_injection_UNION_attack_finding_a_column_containing_text2.png" alt=""><figcaption></figcaption></figure>

* First find out how many columns are in the following table you are using.

<figure><img src="../../../../../.gitbook/assets/SQL_injection_UNION_attack_finding_a_column_containing_text3.png" alt=""><figcaption></figcaption></figure>

* Now to know the writable field, try to go on each column field replacing it with a simple string as the following.
