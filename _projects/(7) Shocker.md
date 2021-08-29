---
name: Shocker
tools: [Perl, Web, Injection]
image: ../img/Shocker_info.png
description: This is Shocker HackTheBox machine walkthrough, this is an easy difficulty linux machine with ip 10.10.10.56.
---

# WriteUp – Shocker – ShellShock

{% include elements/figure.html image="../img/Shocker_info.png" caption="Shocker Info" %}

{% capture list_items %}
Enumeration
Exploitation
Privilege escalation
References
{% endcapture %}
{% include elements/list.html title="Table of Contents" type="toc" %}

```linux
sudo wfuzz -c -t 200 --hc=404 -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt http://10.10.10.56/FUZZ/
```