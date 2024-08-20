# Password Cracking with Rules and Munging

### cewl

Let's say that our user does really likes marvel and because its haves an online website we might be able to use a tool called cewl.

```
cewl https://<website> 
```

### OneRuleToRuleThemAll

* [https://github.com/NotSoSecure/password\_cracking\_rules](https://github.com/NotSoSecure/password\_cracking\_rules)

{% tabs %}
{% tab title="Munged" %}
munge.py -l 9 -i \~/marvel/words -o \~/marvel/munged
{% endtab %}

{% tab title="JohnTheRipper with Rules" %}
john \~/hash --wordlist=munged --rules /opt/OneRuleToRuleThemAll.rule
{% endtab %}
{% endtabs %}
