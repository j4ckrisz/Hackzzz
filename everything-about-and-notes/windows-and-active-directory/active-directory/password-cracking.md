# Password Cracking

{% tabs %}
{% tab title="NTLM" %}
hashcat.exe -m 1000 hashes \<password-list>
{% endtab %}

{% tab title="NTLM v2" %}
hashcat.exe -m 18200 -a 3 hashes.txt rockyou.txt
{% endtab %}
{% endtabs %}
