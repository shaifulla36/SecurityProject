👨‍💻 Author
Shaifulla Hossan
Cybersecurity Enthusiast | Penetration Testing | Red Teaming | Network Security


🔴 Advanced Penetration Testing & Pivoting Lab

A professional cybersecurity home lab built using VMware Workstation, focused on:
 Vulnerability Assessment
 Exploitation
	Privilege Escalation
	Pivoting & Tunneling
	Internal Network Enumeration
	Lateral Movement
	Post-Exploitation
This project simulates a realistic segmented enterprise environment where an attacker compromises an externally exposed host and pivots into an isolated internal network.

🧠 Lab Architecture
External Network — 192.168.50.0/24
	Kali Linux (Attacker Machine)
	Metasploitable 2 (Pivot / Vulnerable Web Server)
Internal Network — 10.10.10.0/24
	Domain Controller
	App Server
	Employee Workstation
Pivot Host
The Metasploitable machine was configured with dual network interfaces:
	eth0 → External Network
	eth1 → Internal Network
This allowed realistic pivoting and internal access simulations.



⚔️ Activities Performed
🔍 Reconnaissance & Enumeration
	Host Discovery (netdiscover, nmap)
	Full Port Scanning
	Service Enumeration
	Vulnerability Identification
	Banner Grabbing

💥 Exploitation
Successfully exploited multiple vulnerable services including:
	vsftpd 2.3.4 Backdoor (CVE-2011-2523)
	Samba usermap_script (CVE-2007-2447)
	PHP CGI Argument Injection (CVE-2012-1823)
	Weak SSH Credentials
	Telnet Brute-force
	MySQL Default Credentials
🛡️ Privilege Escalation
	Meterpreter Session Upgrade
	Token Impersonation
	SYSTEM Privilege Escalation
	LSASS Migration
	NTLM Hash Dumping
🌐 Pivoting & Tunneling
	Meterpreter Autoroute
	SOCKS4a Proxy Configuration
	Proxychains Tunneling
	Internal Network Access Through Pivot Host
🧭 Internal Network Enumeration
	Internal Host Discovery
	Service Enumeration Through Proxychains
	Hidden Subnet Scanning
	Lateral Movement Simulation

🔐 Credential Access
	Hashdump
	John the Ripper
	Hashcat
	Credential Harvesting
🧪 Post Exploitation
	RDP Enablement
	Backdoor User Creation
	Persistence Simulation
	Internal Access Verification

🧰 Tools & Technologies
	Kali Linux
	VMware Workstation
	Metasploit Framework
	Nmap
	Hydra
	Medusa
	Proxychains
	Hashcat
	John the Ripper
	Netdiscover
	Searchsploit
	Meterpreter

📄 Reports Included

This repository contains multiple professional reports covering:
	VMware Lab Setup
	Vulnerability Assessment
	Full Penetration Testing
	Pivoting & Internal Network Access
	Post-Exploitation Workflow

⚠️ Disclaimer
This project was conducted inside a fully isolated and authorized lab environment for educational and research purposes only.
Do NOT use these techniques against systems you do not own or have explicit permission to test.

