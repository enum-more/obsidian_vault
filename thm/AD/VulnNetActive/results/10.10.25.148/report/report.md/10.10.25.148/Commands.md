```bash
nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_quick_tcp_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/xml/_quick_tcp_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -sC --version-all -A --osscan-guess -p- -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_full_tcp_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/xml/_full_tcp_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sU -A --top-ports 100 -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/_top_100_udp_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/xml/_top_100_udp_nmap.xml" 10.10.25.148

dig -p 53 -x 10.10.25.148 @10.10.25.148

dig AXFR -p 53 @10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 53 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp53/tcp_53_dns_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp53/xml/tcp_53_dns_nmap.xml" 10.10.25.148

impacket-getArch -target 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 135 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp135/tcp_135_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp135/xml/tcp_135_rpc_nmap.xml" 10.10.25.148

impacket-rpcdump -port 135 10.10.25.148

enum4linux -a -M -l -d 10.10.25.148 2>&1

nbtscan -rvh 10.10.25.148 2>&1

nmap -vv --reason -Pn -T4 -sV -p 139 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/xml/tcp_139_smb_nmap.xml" 10.10.25.148

smbclient -L //10.10.25.148 -N -I 10.10.25.148 2>&1

smbmap -H 10.10.25.148 -P 139 2>&1

nmap -vv --reason -Pn -T4 -sV -p 445 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/tcp_445_smb_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/xml/tcp_445_smb_nmap.xml" 10.10.25.148

smbmap -H 10.10.25.148 -P 445 2>&1

nmap -vv --reason -Pn -T4 -sV -p 464 --script="banner,krb5-enum-users" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp464/tcp_464_kerberos_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp464/xml/tcp_464_kerberos_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 6379 --script="banner,redis-info" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp6379/tcp_6379_redis_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp6379/xml/tcp_6379_redis_nmap.xml" 10.10.25.148

redis-cli -p 6379 -h 10.10.25.148 INFO

nmap -vv --reason -Pn -T4 -sV -p 49665 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49665/tcp_49665_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49665/xml/tcp_49665_rpc_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 49667 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49667/tcp_49667_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49667/xml/tcp_49667_rpc_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 49669 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49669/tcp_49669_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49669/xml/tcp_49669_rpc_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 49676 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/tcp_49676_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49676/xml/tcp_49676_rpc_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 49687 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49687/tcp_49687_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49687/xml/tcp_49687_rpc_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sV -p 49707 --script="banner,msrpc-enum,rpc-grind,rpcinfo" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49707/tcp_49707_rpc_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp49707/xml/tcp_49707_rpc_nmap.xml" 10.10.25.148

redis-cli -p 6379 -h 10.10.25.148 CONFIG GET '*'

redis-cli -p 6379 -h 10.10.25.148 CLIENT LIST

smbmap -u null -p "" -H 10.10.25.148 -P 445 2>&1

smbmap -H 10.10.25.148 -P 445 -R 2>&1

smbmap -u null -p "" -H 10.10.25.148 -P 445 -R 2>&1

smbmap -H 10.10.25.148 -P 445 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.25.148 -P 139 2>&1

smbmap -u null -p "" -H 10.10.25.148 -P 445 -x "ipconfig /all" 2>&1

smbmap -H 10.10.25.148 -P 139 -R 2>&1

smbmap -u null -p "" -H 10.10.25.148 -P 139 -R 2>&1

smbmap -H 10.10.25.148 -P 139 -x "ipconfig /all" 2>&1

smbmap -u null -p "" -H 10.10.25.148 -P 139 -x "ipconfig /all" 2>&1

dig -p 53 -x 10.10.25.148 @10.10.25.148

dig AXFR -p 53 @10.10.25.148

nmap -vv --reason -Pn -T4 -sU -sV -p 53 --script="banner,(dns* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp53/udp_53_dns_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp53/xml/udp_53_dns_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sU -sV -p 88 --script="banner,krb5-enum-users" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/udp_88_kerberos_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp88/xml/udp_88_kerberos_nmap.xml" 10.10.25.148

nmap -vv --reason -Pn -T4 -sU -sV -p 123 --script="banner,(ntp* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp123/udp_123_ntp_nmap.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp123/xml/udp_123_ntp_nmap.xml" 10.10.25.148


```