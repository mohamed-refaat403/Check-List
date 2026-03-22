# Check-List
A simple Information gathering checklist for penetration testers

# [A] PASSIVE RECON

**[1] Website Recon**:

- About Us
- Contact (Emails, Social media)
- Support
- Careers
- Login

- Partners and third parties
	- Megres and acquisition's, Partnership's, third parties...
	- What type of technologies and system's they use internally?
	- Agiliance site's

- Team member's information's of the website company

- Job search sites
	- Linkedin, Indeed, Monster, Careerbuilder, Glassdoor, Simplyhierd, Fice, Agiliance

======================================

# [2] User infromation Gathering

- Employee's personal information such as:
	- Phone number's, Adresse's, CV, Opinion's, Responsiblitie's, Project's.

- TheHarvester tool
- Infoga tool
- www.pipl.com
- www.peoplefinders.com

======================================

# [3] Search Engines:

- google Hacking Data Base (GHDB)
- The common operator's (AND, OR, +, -, "")

* You can try to search with website signature in google dorc's

- Evil dorc's (google hacking database)
- Foca tool (Windows only)
- Web archive

======================================

# [4] Whois Enumeration:

* Used for querying an official domain registrar's database, in order to determine
* The owner of a domain name
* Ip address or range
* Technical contact's
* Expiration date of the domain

- who.is
- whois.domaintools.com
- bgp.he.net
- networking.ringofsaturn.com
- betterwhois.com
- viewdns.info

* Classless Inter-Domain Routing (CIDR)
-هو range ال ip's اللي بتاخده الشركة من ال ISP
	- Ex: 163.114.128.0/24
	
* An Autonomous System Number (ASN)
	- Ex: AS54115

======================================

**[5] Subdomain Enumeration:**

- Tools:
	- Sublister
	- Amass

======================================

**[6] OpenSource code:**

- Manual:
	- Github:
		- "Company" password
		- "Company" secret
		- "Company" credential's
		- "Company" token
		- "Company" config
		- "Company" key
		- "Company" pass
		- "Company" login
		- "Company" ftp
		- "Company" pwd
		- "Company" security_credential's	#LDAB (AD)
		- "Company" connectionstring		#DATA Base
		- "Company" JDBC					#DATA Base 
		- "Company" ssh_auth_password
		- "Company" send_key, send,key's

	- StackOverFlow

- Scripts:
	- Gitrob
	- Gitleaks

======================================

**[7] Shodan & Censys.io:**

* Any device connected to the internet:
	* server's, router's, IoT device's

- Using Dorks in shodan:
	- hostname: uber.com

======================================

**[8] Pastebin & Have i been pwned:**
	* To search for data breashes

======================================

**[9] Osint Framework & Maltego:**

======================================

# [B] Active RECON 

[1] DNS Enumeration:

* What is DNS?

- Interacting with a DNS Server:
	- Forward lookup:
		- A (Record):
			* Map's a hostname to an ip, "forward" lookup/ zone.

	- Reverse lookup:
		- PTR:
			* Map's an ip to a hostname, "reverse" lookup/ zone.

	- CNAME:
		* Map's an alias hostname to an A record hostname.

	- MX:
		* contain the name's of the server's resposible for handling email forthe domain.
		* A domain can contain multiple MX revord's.

- Forward lookup Brute Force:
	- Host -r A <domain name>

- Reverse Lookup Brute Force:
	- host -t PTR <ip>

- DNS Zone Transfer's:
	- Full dump of the zone file's.
	- host -l <domain name> <dns server address>

- Automate:
	- dnsrecon (tool)
	- dnsenum (tool)

======================================

[2] Port Scaning:

- Tcp Scanning:
	- nc -nvv -w 1 -z <target ip> <ip range>

- Udp Scanning:
	- nc -nvv -u -w 1 -z <target ip> <ip range>

======================================

[3] Nmap:

* Accountability for our Traffic's

- TCP connect scan

- Stealth scan

- Network Sweeping:
	* nmap -sn <range-254> -V

- OS Fingerprinting:
	* sudo nmap -O <host>
	* the "ttl" from ICMP ping refers for the OS type

- Banner Grabbing/ Service Enumeration:
	* sudo nmap <host> -sV #service vertion

- Nmap Scripting Engien's (NSE)

======================================

[4] Masscan

======================================

[5] SMB Enumeration:
 
- Scanning for the NetBIOS & SMB Service:
	- nbtscan (tool)
	- smbclient (tool)
	- smbmap (tool)
	- enum4linux (tool)
	- nmap SMB script's

======================================

[6] NFS Enumeration:

- Nmap NFS NSE Script's
- rpcinfo (tool) + showmount (tool)

======================================

**[7] SMTP Enumeration:**

======================================

[8] SNMP Enumeration:

* Check the MID & OID before diving into SNMP enum

- Scanning for the SNMP Service:
	- nmap
	- metasploit
	- snmpwalk
	- snmpset (for Exploitation)



