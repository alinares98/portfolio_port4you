---
name: Shocker
tools: [Perl, Web, Injection]
image: ../img/Shocker_info.png
description: This is Shocker HackTheBox machine walkthrough, this is an easy difficulty linux machine with ip 10.10.10.56.
---

# WriteUp – Shocker – ShellShock

{% include elements/figure.html image="../img/Shocker/Shocker_info.png" %}

Today we are going to make the [HackTheBox](https://www.hackthebox.eu/) 
**Shocker** machine, it is a very simple machine but it will allow us 
to know more about the **ShellShock** vulnerability that we will see later.

#Enumeration

First of all, a port scan will be executed with **Nmap** in order to see which 
ports are open on the target machine.

```
sudo nmap -p- -sS --min-rate 5000 --open  -vvv -n -Pn 10.10.10.56 -oG allPorts
```
{% include elements/figure.html image="../img/Shocker/ports_nmap.png" %}

* `-p-`
- `-sS-`
+ `--min-rate 5000`
- `--open`
- `-vvv`
- `-n`
- `-Pn`
- `-oG`


{% capture list_items %}
Enumeration
Exploitation
Privilege escalation
References
{% endcapture %}
{% include elements/list.html title="Table of Contents" type="toc" %}
