```bash
nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_full_tcp_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/xml/_full_tcp_nmap.xml" 10.10.25.148
```

[/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_full_tcp_nmap.txt](file:///root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_full_tcp_nmap.txt):

```
# Nmap 7.92 scan initiated Thu Jul 14 20:55:16 2022 as: nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_full_tcp_nmap.txt -oX /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/xml/_full_tcp_nmap.xml 10.10.25.148
Nmap scan report for 10.10.25.148
Host is up, received user-set (0.19s latency).
Scanned at 2022-07-14 20:55:17 IST for 383s
Not shown: 65521 filtered tcp ports (no-response)
PORT      STATE SERVICE       REASON          VERSION
53/tcp    open  domain        syn-ack ttl 127 Simple DNS Plus
135/tcp   open  msrpc         syn-ack ttl 127 Microsoft Windows RPC
139/tcp   open  netbios-ssn   syn-ack ttl 127 Microsoft Windows netbios-ssn
445/tcp   open  microsoft-ds? syn-ack ttl 127
464/tcp   open  kpasswd5?     syn-ack ttl 127
6379/tcp  open  redis         syn-ack ttl 127 Redis key-value store 2.8.2402
9389/tcp  open  mc-nmf        syn-ack ttl 127 .NET Message Framing
49665/tcp open  msrpc         syn-ack ttl 127 Microsoft Windows RPC
49667/tcp open  msrpc         syn-ack ttl 127 Microsoft Windows RPC
49669/tcp open  msrpc         syn-ack ttl 127 Microsoft Windows RPC
49670/tcp open  ncacn_http    syn-ack ttl 127 Microsoft Windows RPC over HTTP 1.0
49676/tcp open  msrpc         syn-ack ttl 127 Microsoft Windows RPC
49687/tcp open  msrpc         syn-ack ttl 127 Microsoft Windows RPC
49707/tcp open  msrpc         syn-ack ttl 127 Microsoft Windows RPC
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
OS fingerprint not ideal because: Missing a closed TCP port so results incomplete
No OS matches for host
TCP/IP fingerprint:
SCAN(V=7.92%E=4%D=7/14%OT=53%CT=%CU=%PV=Y%DS=2%DC=T%G=N%TM=62D036DC%P=aarch64-unknown-linux-gnu)
SEQ(SP=106%GCD=1%ISR=109%TI=I%II=I%SS=S%TS=U)
OPS(O1=M505NW8NNS%O2=M505NW8NNS%O3=M505NW8%O4=M505NW8NNS%O5=M505NW8NNS%O6=M505NNS)
WIN(W1=FFFF%W2=FFFF%W3=FFFF%W4=FFFF%W5=FFFF%W6=FF70)
ECN(R=Y%DF=Y%TG=80%W=FFFF%O=M505NW8NNS%CC=Y%Q=)
T1(R=Y%DF=Y%TG=80%S=O%A=S+%F=AS%RD=0%Q=)
T2(R=N)
T3(R=N)
T4(R=N)
U1(R=N)
IE(R=Y%DFI=N%TG=80%CD=Z)

Network Distance: 2 hops
TCP Sequence Prediction: Difficulty=262 (Good luck!)
IP ID Sequence Generation: Incremental
Service Info: OS: Windows; CPE: cpe:/o:microsoft:windows

Host script results:
|_clock-skew: 0s
| smb2-security-mode: 
|   3.1.1: 
|_    Message signing enabled and required
| smb2-time: 
|   date: 2022-07-14T15:31:03
|_  start_date: N/A
| p2p-conficker: 
|   Checking for Conficker.C or higher...
|   Check 1 (port 5738/tcp): CLEAN (Timeout)
|   Check 2 (port 21579/tcp): CLEAN (Timeout)
|   Check 3 (port 60176/udp): CLEAN (Timeout)
|   Check 4 (port 45747/udp): CLEAN (Timeout)
|_  0/4 checks are positive: Host is CLEAN or ports are blocked

TRACEROUTE (using port 135/tcp)
HOP RTT       ADDRESS
1   187.06 ms 10.11.0.1
2   187.52 ms 10.10.25.148

Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Thu Jul 14 21:01:40 2022 -- 1 IP address (1 host up) scanned in 384.37 seconds

```
