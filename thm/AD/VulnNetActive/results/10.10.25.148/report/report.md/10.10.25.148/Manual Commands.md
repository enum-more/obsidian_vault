```bash
[*] domain on tcp/53

	[-] Use dnsrecon to bruteforce subdomains of a DNS domain.

		dnsrecon -n 10.10.25.148 -d <DOMAIN-NAME> -D /usr/share/seclists/Discovery/DNS/subdomains-top1million-110000.txt -t brt 2>&1 | tee /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp53/tcp_53_dnsrecon_subdomain_bruteforce.txt

	[-] Use dnsrecon to automatically query data from the DNS server. You must specify the target domain name.

		dnsrecon -n 10.10.25.148 -d <DOMAIN-NAME> 2>&1 | tee /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp53/tcp_53_dnsrecon_default_manual.txt

[*] msrpc on tcp/135

	[-] RPC Client:

		rpcclient -p 135 -U "" 10.10.25.148

[*] netbios-ssn on tcp/139

	[-] Nmap scans for SMB vulnerabilities that could potentially cause a DoS if scanned (according to Nmap). Be careful:

		nmap -vv --reason -Pn -T4 -sV -p 139 --script="smb-vuln-ms06-025" --script-args="unsafe=1" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_ms06-025.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/xml/tcp_139_smb_ms06-025.xml" 10.10.25.148

		nmap -vv --reason -Pn -T4 -sV -p 139 --script="smb-vuln-ms07-029" --script-args="unsafe=1" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_ms07-029.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/xml/tcp_139_smb_ms07-029.xml" 10.10.25.148

		nmap -vv --reason -Pn -T4 -sV -p 139 --script="smb-vuln-ms08-067" --script-args="unsafe=1" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/tcp_139_smb_ms08-067.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp139/xml/tcp_139_smb_ms08-067.xml" 10.10.25.148

[*] microsoft-ds on tcp/445

	[-] Lookup SIDs

		lookupsid.py [username]:[password]@10.10.25.148

	[-] Nmap scans for SMB vulnerabilities that could potentially cause a DoS if scanned (according to Nmap). Be careful:

		nmap -vv --reason -Pn -T4 -sV -p 445 --script="smb-vuln-ms06-025" --script-args="unsafe=1" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/tcp_445_smb_ms06-025.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/xml/tcp_445_smb_ms06-025.xml" 10.10.25.148

		nmap -vv --reason -Pn -T4 -sV -p 445 --script="smb-vuln-ms07-029" --script-args="unsafe=1" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/tcp_445_smb_ms07-029.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/xml/tcp_445_smb_ms07-029.xml" 10.10.25.148

		nmap -vv --reason -Pn -T4 -sV -p 445 --script="smb-vuln-ms08-067" --script-args="unsafe=1" -oN "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/tcp_445_smb_ms08-067.txt" -oX "/root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/tcp445/xml/tcp_445_smb_ms08-067.xml" 10.10.25.148

[*] msrpc on tcp/49665

	[-] RPC Client:

		rpcclient -p 49665 -U "" 10.10.25.148

[*] msrpc on tcp/49667

	[-] RPC Client:

		rpcclient -p 49667 -U "" 10.10.25.148

[*] msrpc on tcp/49669

	[-] RPC Client:

		rpcclient -p 49669 -U "" 10.10.25.148

[*] msrpc on tcp/49676

	[-] RPC Client:

		rpcclient -p 49676 -U "" 10.10.25.148

[*] msrpc on tcp/49687

	[-] RPC Client:

		rpcclient -p 49687 -U "" 10.10.25.148

[*] msrpc on tcp/49707

	[-] RPC Client:

		rpcclient -p 49707 -U "" 10.10.25.148

[*] domain on udp/53

	[-] Use dnsrecon to bruteforce subdomains of a DNS domain.

		dnsrecon -n 10.10.25.148 -d <DOMAIN-NAME> -D /usr/share/seclists/Discovery/DNS/subdomains-top1million-110000.txt -t brt 2>&1 | tee /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp53/udp_53_dnsrecon_subdomain_bruteforce.txt

	[-] Use dnsrecon to automatically query data from the DNS server. You must specify the target domain name.

		dnsrecon -n 10.10.25.148 -d <DOMAIN-NAME> 2>&1 | tee /root/enum-more/obsidian_vault/VulnNetActive/results/10.10.25.148/scans/udp53/udp_53_dnsrecon_default_manual.txt


```