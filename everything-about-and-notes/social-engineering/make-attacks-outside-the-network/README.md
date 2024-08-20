# Make attacks outside the network



<figure><img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Flearn.g2crowd.com%2Fhubfs%2FPort%2520Forwarding%252003.png&#x26;f=1&#x26;nofb=1&#x26;ipt=fb7102fbefb6c32e84a686e2cbf3365e8eebb45c8cfd9ccfa29a758c6b7e2475&#x26;ipo=images" alt=""><figcaption></figcaption></figure>

This section will focus on what it is port forwarding and how to be configured well.

* Here you see how port forwarding works, and we will be doing something similar to that.

1. The _**source (Desktop)**_ is sending a packet to the _**Destination (server)**_ and is making a request throw port _**443**_.
2. But the packet needs to arrive first to the router so the router can send the _**Desktop**_ packet to the _**destination**_. How? With _**Network Address Translation (NAT)**_ we can use a **Private IP** Address millions of times all over the world inside our networks and still we can access to the Internet. Here, NAT provides the translation from Private IP Address to the **Public IP** Address. We are connecting Internet with our **Private IP Address**, but in real at the backplane, our router is connecting Internet via **Public IP Address**.
3. So, the packet arrive to the server and the server responds back.
