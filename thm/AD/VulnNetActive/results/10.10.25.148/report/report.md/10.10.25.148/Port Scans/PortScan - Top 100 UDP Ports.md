```bash
nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_top_100_udp_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/xml/_top_100_udp_nmap.xml" 10.10.25.148
```

[/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_top_100_udp_nmap.txt](file:///root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_top_100_udp_nmap.txt):

```
# Nmap 7.92 scan initiated Thu Jul 14 20:55:16 2022 as: nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_top_100_udp_nmap.txt -oX /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/xml/_top_100_udp_nmap.xml 10.10.25.148
Nmap scan report for 10.10.25.148
Host is up, received user-set (0.23s latency).
Scanned at 2022-07-14 20:55:17 IST for 1770s
Not shown: 97 open|filtered udp ports (no-response)
PORT    STATE SERVICE      REASON               VERSION
53/udp  open  domain       udp-response ttl 127 (generic dns response: SERVFAIL)
| fingerprint-strings: 
|   NBTStat: 
|_    CKAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
88/udp  open  kerberos-sec udp-response         Microsoft Windows Kerberos (server time: 2022-07-14 15:25:32Z)
123/udp open  ntp          udp-response ttl 127 NTP v3
| ntp-info: 
|_  receive time stamp: 2022-07-14T15:32:07
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port53-UDP:V=7.92%I=7%D=7/14%Time=62D0357B%P=aarch64-unknown-linux-gnu%
SF:r(NBTStat,32,"\x80\xf0\x80\x82\0\x01\0\0\0\0\0\0\x20CKAAAAAAAAAAAAAAAAA
SF:AAAAAAAAAAAAA\0\0!\0\x01");
Too many fingerprints match this host to give specific OS details
TCP/IP fingerprint:
SCAN(V=7.92%E=4%D=7/14%OT=%CT=%CU=%PV=Y%DS=2%DC=T%G=N%TM=62D03C47%P=aarch64-unknown-linux-gnu)
SEQ(II=I)
U1(R=N)
IE(R=Y%DFI=N%TG=80%CD=Z)

Network Distance: 2 hops
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: 3s

TRACEROUTE (using port 123/udp)
HOP RTT       ADDRESS
1   183.50 ms 10.11.0.1
2   307.77 ms 10.10.25.148

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Thu Jul 14 21:24:47 2022 -- 1 IP address (1 host up) scanned in 1770.48 seconds

```
