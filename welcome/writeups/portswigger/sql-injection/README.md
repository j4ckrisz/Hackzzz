---
description: https://portswigger.net/web-security/sql-injection
---

# 💉 SQL Injection

## Intro to SQL Injection

* Is a web security vulnerability that allows an attacker to interfere with the queries that an application makes to its database.
* It generally allows an attacker to **view data that they are not normally able to retrieve.**
* This might include **data belonging to other users**, or any other **data that the application itself is able to access.** In many cases, an attacker can **modify** or **delete this data**, causing persistent changes to the application's content or behavior.
* In some situations, an attacker can escalate an SQL injection attack to compromise the **underlying server or other back-end infrastructure or perform a denial-of-service attack.**

## What's the impact of SQLi?

* _**Many high-profile data breaches in recent years have been the result of SQL injection attacks**_, leading to reputational damage and regulatory fines.
* In some cases, _**an attacker can obtain a persistent backdoor into an organization's systems, leading to a long-term compromise that can go unnoticed for an extended period.**_
