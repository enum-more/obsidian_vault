---
title: "THM - # VulnNet: Active"
classes: wide
header:
  teaser: /assets/images/htb/htb.png
ribbon: blue
description: "Writeup for THM - # VulnNet: Active"
categories:
  - THM
---

The given box ```VulnNet: Active``` is a Linux machine with an IP address of ```10.10.135.22```

- [TryHackMe- VulnNet:Active](#tryhackme---razorblack)
  - [Recon](#recon)
    - [Nmap Scan Result](#nmap-scan-result)
  - [Enumeration](#enumeration)
    - [RPC](#rpc)
    	- [usernames](#usernames)
    	- [AD username format ](#AD-username-format)
    	- [Request AS_REP message](#Request-AS_REP-message)
    	- [Cracking the hash](#Cracking-the-hash)
  

## Recon

### Nmap Scan Result