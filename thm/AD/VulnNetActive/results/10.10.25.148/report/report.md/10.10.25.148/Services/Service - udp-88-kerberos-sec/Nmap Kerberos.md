```bash
nmap -vv --reason -Pn -T4 -sU -sV -p 88 --script="banner,krb5-enum-users" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/udp_88_kerberos_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/xml/udp_88_kerberos_nmap.xml" 10.10.25.148
```

[/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/udp_88_kerberos_nmap.txt](file:///root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/udp_88_kerberos_nmap.txt):

```
# Nmap 7.92 scan initiated Thu Jul 14 21:24:47 2022 as: nmap -vv --reason -Pn -T4 -sU -sV -p 88 --script=banner,krb5-enum-users -oN /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/udp_88_kerberos_nmap.txt -oX /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/xml/udp_88_kerberos_nmap.xml 10.10.25.148
Nmap scan report for 10.10.25.148
Host is up, received user-set.
Scanned at 2022-07-14 21:24:47 IST for 7s

PORT   STATE SERVICE      REASON       VERSION
88/udp open  kerberos-sec udp-response Microsoft Windows Kerberos (server time: 2022-07-14 15:54:53Z)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Thu Jul 14 21:24:54 2022 -- 1 IP address (1 host up) scanned in 6.66 seconds

```
