# Drone Hacking

I was wondering for a while, **how can I hack a drone**, my question was, **a drone could be hackable?** The answer is **yes** and is simpler than you might think.

## What's the concept?

Nowadays **literally every drone is controlled via a **_**Wi-Fi connection**_, when you power on your drone starts an _**Access Point**_ to connect to it.&#x20;

The **majority of this AP's **_**doesn't require a password**_ to connect to it, that means if an attacker wants to have connectivity with the drone, he just need to connect to their AP to communicate with the drone.

Knowing that, we just need to see how to get in the drone system. **Hak5 once again make it possible,** with the **Wi-Fi pineapple, you can do a cyber weapon attaching the Wi-Fi pineapple to the drone.**

### How to know who AP connect?

The Drone Access Point Name is related with the **MAC address** of the drone, so like we see in the video you can make a script that parse this and connects to it to further exploitation.

### How to get into the drone

You can do like in the video play with the **empty** command that is like a **expect** to interact with the drone and telnet to it doing a **BusyBox** command to **get a shell**.

{% embed url="https://www.youtube.com/watch?v=xKfY0PmKDRE" %}

