# plink

<pre class="language-java"><code class="lang-java">// Example
cmd.exe /c echo y | .\plink.exe -R 8000:172.16.0.10:80 kali@172.16.0.20 -i KEYFILE -N
<strong>
</strong><strong>// Remember to change ssh-keygen
</strong>puttygen KEYFILE -o OUTPUT_KEY.ppk
</code></pre>
