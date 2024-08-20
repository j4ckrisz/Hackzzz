---
cover: >-
  https://images.unsplash.com/photo-1633419461186-7d40a38105ec?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHNlYXJjaHwyfHx3aW5kb3dzJTIwb3N8ZW58MHx8fHwxNjg4MDA5NDI2fDA&ixlib=rb-4.0.3&q=85
coverY: 0
---

# Active Directory

## **What is active directory?**

* **Directory service developed by Microsoft to manage Windows Domain Networks.**
* **Stores Information related to objects, such as Computers, users, Printers, etc.**
* **Authenticates using kerberos tickets.**

## **Why Active Directory?**

**Active Directory lets you create security groups, setting up which users can access which network assets, such as shared files and applications.**&#x20;

You can also organize your company’s network hierarchy. For example, it’s through AD that you determine which computers and printers belong on the network**.**

&#x20;**Active Directory is the most commonly used identity management service in the world.**&#x20;

## **Active Directory Physical Components**

### Domain Controller's

This is a server with **AD DS server role** installed that has specifically been promoted to a domain controller.

#### What it does?

* Host a copy of the **AD DS** directory store
* Provide **authentication** and **authorization** services&#x20;
* **Replicate Updates** to other Domain Controllers in the **Domain Forest**
* **Allow** administrative access to manage **user account** and **network resources**

## What the AD DS?

The **Active Directory Data Store** contains some **database files**, **manage user information or even processes, services and application.**

* Consist of the database file **Ntds.dit** **(aka: The Most Famous DB File in Active Directory)**
* Is store by default in the **%Systemroot%\NTDS** folder in the Domain Controllers
* The **Ntds.dit** file include a lot of **sensitive information** like, **users, passwords, objects**, etc.

<figure><img src="https://th.bing.com/th/id/R.1809465f90c361b68124bf42cfbd9c7a?rik=dSDO51OlAMwLgw&#x26;riu=http%3a%2f%2fpowershell-guru.com%2fwp-content%2fuploads%2f2015%2f11%2fntds-dit-active-directory.png&#x26;ehk=o7HLmA4h15tHAcKtYukf8azY6ntdTVaip5KxOZm0KIA%3d&#x26;risl=&#x26;pid=ImgRaw&#x26;r=0" alt=""><figcaption></figcaption></figure>

## Domains

Contains all the information about the objects of the Active directory. Domains are used to group and manage objects in organization.

* The **objects** of the directory are contained inside the **domain**. Inside a "**forest**" more than one domain can exist and each of them will have their own **objects collection**.
* Is just one domain **(Example: enterprise.com)**

## **Trees**

&#x20;Group of domains with the same root. **(Example: **_**dom.local, email.dom.local, www.dom.local)**_

<figure><img src="https://image2.slideserve.com/4321219/2-domain-trees-l.jpg" alt=""><figcaption></figcaption></figure>

## Forest

Is just a **collection** of **Trees, it could be more than one**.&#x20;

<figure><img src="https://th.bing.com/th/id/R.f2c81524be7bc6a9688139266446c424?rik=K3eoT%2fK6dplyKw&#x26;riu=http%3a%2f%2fwww.omnisecu.com%2fimages%2fwindows-2003%2factive-directory%2factive-directory-forest.gif&#x26;ehk=2NQvlVa%2bJlm9UAGC1WjzacWUKNU8Fm0NcC4AM57DqOc%3d&#x26;risl=&#x26;pid=ImgRaw&#x26;r=0&#x26;sres=1&#x26;sresct=1" alt=""><figcaption></figcaption></figure>

* Share a common **configuration partition.**
* Enable **trust** between **all domains in the forest.**
* **Admins** and **Schema admin groups** are shared.

## Organizational Units (OU's)

Containers that can have, users, groups, computers etc.

<figure><img src="https://www.tech-faq.com/wp-content/uploads/active-directory-organizational-units.jpg" alt=""><figcaption></figcaption></figure>

* Apply Policies, delegate permissions to admin group of objects and manage.

## Domain Trust

Microsoft considers that the **domain isn't a Security Boundary**, the **Forest is the security Boundary**. This means that **if you compromise a domain inside a Forest, you might be able to compromise the entire Forest**.

<figure><img src="https://image.slidesharecdn.com/activedirectorydomainandtrust-161018173334/95/slide-3-1024.jpg" alt=""><figcaption></figcaption></figure>

## Objects

There are **7 objects** that you need to know.

{% tabs %}
{% tab title="Printers" %}
Simplify connecting and locating printers
{% endtab %}

{% tab title="Users" %}
Network resource access
{% endtab %}

{% tab title="Groups" %}
&#x20;Simplify administrator control.
{% endtab %}

{% tab title="Shared Folder" %}
User can search for shared folders based on the properties.
{% endtab %}

{% tab title="Contacts" %}
Used to assign e-mail address to external users.
{% endtab %}

{% tab title="InetOrgPerson" %}
Compatibility with other directory services.
{% endtab %}

{% tab title="Computers" %}
Management of resources like, authentication, auditing users, access and resources.
{% endtab %}
{% endtabs %}

## Resources

* [ ] Microsoft: [https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/active-directory-domain-services](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/active-directory-domain-services)
* [ ] Hacktrickz Active Directory: [https://book.hacktricks.xyz/windows-hardening/active-directory-methodology](https://book.hacktricks.xyz/windows-hardening/active-directory-methodology)

