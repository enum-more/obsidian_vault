```bash
nmap -vv --reason -Pn -T4 -sV -p 49676 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/tcp_49676_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/xml/tcp_49676_rpc_nmap.xml" 10.10.25.148
```

[/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/tcp_49676_rpc_nmap.txt](file:///root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/tcp_49676_rpc_nmap.txt):

```
# Nmap 7.92 scan initiated Thu Jul 14 21:01:41 2022 as: nmap -vv --reason -Pn -T4 -sV -p 49676 --script=banner,msrpc-enum,rpc-grind,rpcinfo -oN /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/tcp_49676_rpc_nmap.txt -oX /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/xml/tcp_49676_rpc_nmap.xml 10.10.25.148
Nmap scan report for 10.10.25.148
Host is up, received user-set (0.21s latency).
Scanned at 2022-07-14 21:01:43 IST for 72s

PORT      STATE SERVICE REASON          VERSION
49676/tcp open  msrpc   syn-ack ttl 127 Microsoft Windows RPC
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Thu Jul 14 21:02:55 2022 -- 1 IP address (1 host up) scanned in 74.05 seconds

```
