```bash
nmap -vv --reason -Pn -T4 -sV -p 139 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/xml/tcp_139_smb_nmap.xml" 10.10.25.148
```

[/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_nmap.txt](file:///root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_nmap.txt):

```
# Nmap 7.92 scan initiated Thu Jul 14 21:01:41 2022 as: nmap -vv --reason -Pn -T4 -sV -p 139 "--script=banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_nmap.txt -oX /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/xml/tcp_139_smb_nmap.xml 10.10.25.148
Nmap scan report for 10.10.25.148
Host is up, received user-set (0.20s latency).
Scanned at 2022-07-14 21:01:42 IST for 43s

PORT    STATE SERVICE     REASON          VERSION
139/tcp open  netbios-ssn syn-ack ttl 127 Microsoft Windows netbios-ssn
|_smb-enum-services: ERROR: Script execution failed (use -d to debug)
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_smb-print-text: false
|_smb2-time: ERROR: Script execution failed (use -d to debug)
|_smb-vuln-ms10-061: SMB: Couldn't find a NetBIOS name that works for the server. Sorry!
|_smb2-security-mode: SMB: Couldn't find a NetBIOS name that works for the server. Sorry!
|_smb2-capabilities: SMB: Couldn't find a NetBIOS name that works for the server. Sorry!
|_smb-protocols: No dialects accepted. Something may be blocking the responses
|_smb-mbenum: ERROR: Script execution failed (use -d to debug)

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Thu Jul 14 21:02:25 2022 -- 1 IP address (1 host up) scanned in 44.32 seconds

```
