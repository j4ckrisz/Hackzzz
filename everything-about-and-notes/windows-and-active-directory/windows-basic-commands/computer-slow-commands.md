# Computer Slow Command's

{% tabs %}
{% tab title="chkdsk" %}
chkdsk /f -> **will see if there's any errors.**

chkdsk /r **-> Check for issues and fix them**.
{% endtab %}

{% tab title="sfc" %}
sfc /scannow **-> Check system files and if they are bad it will fix them or replace them.**
{% endtab %}

{% tab title="DISM" %}
DISM /online /Cleanup-Image /scanhealth **-> This will fix your system image**

DISM /online /Cleanup-Image /restorehealth
{% endtab %}
{% endtabs %}
