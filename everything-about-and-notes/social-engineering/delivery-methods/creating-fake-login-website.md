# Creating Fake Login Website

## Download The Login Page

* In order to clone a website login, use _**Webscrapbook**_ to download all the login page and save it in a folder.

<figure><img src="../../../.gitbook/assets/webscrapbook.png" alt=""><figcaption></figcaption></figure>

* Download a login page click on the webscrapbook logo and click in _**Capture Tabs (Source)**_.

<figure><img src="../../../.gitbook/assets/webscrapbook2.png" alt=""><figcaption></figcaption></figure>

* Now that you downloaded the login page go to the folder you save it and try it with **php 0.0.0.0:80** to see if everything it's downloaded correctly.

<figure><img src="../../../.gitbook/assets/webscrap3.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/webscrap4.png" alt=""><figcaption></figcaption></figure>

* Here you can see the login page in my local machine.

## Setting The Credential Harvester with (Setoolkit)

* Type **setoolkit** to run it.&#x20;

<figure><img src="../../../.gitbook/assets/setoolkit.png" alt=""><figcaption></figcaption></figure>

* Choose the option 1

<figure><img src="../../../.gitbook/assets/setoolkit2.png" alt=""><figcaption></figcaption></figure>

* Choose the option 2

<figure><img src="../../../.gitbook/assets/setoolkit3.png" alt=""><figcaption></figcaption></figure>

* Choose the option 3

<figure><img src="../../../.gitbook/assets/set_set.png" alt=""><figcaption></figcaption></figure>

* Now here you will configure the credential harvester.
* Pass your **IP,** set the route where you have downloaded the login website, and set the option 2.
* Finally copy the original URL of the website and paste it.

<figure><img src="../../../.gitbook/assets/webscrapbook5.png" alt=""><figcaption></figcaption></figure>

* Now our fake login website is working, if we send this to somebody it will see this and once, they put their credentials we will see it from the terminal.

<figure><img src="../../../.gitbook/assets/webscrapbook6.png" alt=""><figcaption></figcaption></figure>

* As our last step, now we can send this to our targets.
