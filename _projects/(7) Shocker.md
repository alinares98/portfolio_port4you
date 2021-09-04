---
name: Shocker
tools: [Perl, Web, Injection]
image: ../img/Shocker/Shocker_info.png
description: This is Shocker HackTheBox machine walkthrough, this is an easy difficulty linux machine with ip 10.10.10.56.
---

# WriteUp – Shocker – ShellShock

{% include elements/figure.html image="../img/Shocker/Shocker_info.png" %}

Today we are going to make the [HackTheBox](https://www.hackthebox.eu/) 
**Shocker** machine, it is a very simple machine but it will allow us 
to know more about the **ShellShock** vulnerability that we will see later.

{% capture list_items %}
Enumeration
Exploitation
Privilege escalation
References
{% endcapture %}
{% include elements/list.html title="Table of Contents" type="toc" %}

# Enumeration

First of all, a port scan will be executed with **Nmap** in order to see which 
ports are open on the target machine.

```
sudo nmap -p- -sS --min-rate 5000 --open  -vvv -n -Pn 10.10.10.56 -oG allPorts
```
{% include elements/figure.html image="../img/Shocker/nmap_ports.png" %}

* `-p-` To scan all ports from 1 to 65535
- `-sS-` TCP SYN scan 
+ `--min-rate 5000` Scanning speed 5000 packets per second
- `--open` Show only open (or possibly open) ports
- `-vvv` Increases the verbosity level, causing Nmap to print more information about the scan in progress
- `-n` No DNS resolution
- `-Pn` This option skips the host discovery stage altogether 
- `-oG` Grepable output


[More info](https://explainshell.com/explain?cmd=sudo+nmap+-p-+-sS+--min-rate+5000+--open++-vvv+-n+-Pn+10.10.10.56+-oG+allPorts)

Now, nmap is going to be used again, in this case to determine which services 
and versions are running on the ports that were obtained earlier.

```
sudo nmap -sC -sV -p80,2222 10.10.10.56 -oN targeted
```


* `-sC` Performs a script scan using the default set of scripts
- `-sV` Enables version detection
+ `-oN` Normal output

[More info](https://explainshell.com/explain?cmd=sudo+nmap+-sC+-sV+-p80%2C2222+10.10.10.56+-oN+targeted)
