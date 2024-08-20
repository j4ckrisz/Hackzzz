# Network Command's

### Basic Network Commands

{% tabs %}
{% tab title="ipconfig" %}
ipconfig /all **-> show all network info.**

ipconfig /release **-> release all matching connections.**

ipconfig /displaydns **-> displays dns cache information.**

ipconfig /flushdns **-> deletes the dns cache.**
{% endtab %}

{% tab title="nslookup" %}
nslookup -type=google.com **-> it will tell you what dns server you're using, and the answer is giving.**

nslookup - google.com 8.8.8.8 **-> You can try to specify the dns like this.**
{% endtab %}

{% tab title="route" %}
route print **-> show the routing table of your computer.**
{% endtab %}

{% tab title="ping" %}
ping 8.8.8.8 **-> Check internet connection by pining google's dns.**

ping -t \<website> **-> this will never stop.**
{% endtab %}

{% tab title="tracert" %}
tracert \<website> **-> trace the path to your website.**
{% endtab %}

{% tab title="netstat" %}
netstat -af **-> What ports are open.**

netstat -o **-> Show PID of the process running in the port.**

netstat -nat **-> Show all active connections.**
{% endtab %}

{% tab title="netsh" %}
netsh wlan show wlan report **-> gives a super fancy report about your wireless interfaces.**

netsh interface show interface **-> show you interfaces.**

netsh interface ip show address | findstr "IP address" **-> Quick one liner to find all interface ip address.**

netsh interface ip show dnsservers  **-> dns server ip.**

netsh advfirewall set allprofiles state off **-> turn firewall on/off.**
{% endtab %}
{% endtabs %}
