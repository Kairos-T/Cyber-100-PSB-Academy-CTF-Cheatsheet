
## Footprinting and Reconnaissance

- `whois`: Queries the WHOIS database to find information about domain name registration.
  - Syntax: `whois <domain>`
  - Example: `whois google.com`
- `dnsenum`: Gathers information about a target's DNS, such as the IP addresses of DNS servers, mail servers, and other hosts associated with the domain.
  - Syntax: `dnsenum <domain>`
  - Example: `dnsenum example.com`
- `theHarvester`: [Gathers emails, subdomains, hosts, employee names, open ports and banners from different public sources.]()
  - Syntax: `theHarvester -d <domain> -b <search engine>`
  - Example: `theHarvester -d microsoft.com -b google`
- `netdiscover`: Discovers hosts on a local network.
  - Syntax: `netdiscover -r <IP range>`
  - Example: `netdiscover -r 192.168.1.0/24`
- `nmap`: Scans hosts and services on a network, and discovers vulnerabilities.
  - Syntax: `nmap -sS <IP or hostname>`
  - Example: `nmap -sS 192.168.1.1`
- `recon-ng`: A full-featured Web Reconnaissance framework written in Python.
  - Syntax: `recon-ng`
  - Example: `recon-ng`

## Scanning Networks

- `nmap`: Scans hosts and services on a network, and discovers vulnerabilities.
  - Syntax: `nmap -p <port> <IP or hostname>`
  - Example: `nmap -p 80 192.168.1.1`
- `masscan`: A high-speed scanner for large-scale TCP/IP port scanning.
  - Syntax: `masscan -p <port> <IP range>`
  - Example: `masscan -p 22,80 192.168.1.0/24`
- `unicornscan`: A stateless network scanner that can scan multiple hosts simultaneously.
  - Syntax: `unicornscan -mT <IP or hostname>`
  - Example: `unicornscan -mT 192.168.1.1`
- `zmap`: A fast single-packet network scanner designed for Internet-wide network surveys.
  - Syntax: `zmap -p <port> <IP range>`
  - Example: `zmap -p 80 192.168.1.0/24`

## Vulnerability Analysis

- `nmap`: Scans hosts and services on a network, and discovers vulnerabilities.
  - Syntax: `nmap --script=<script name> <IP or hostname>`
  - Example: `nmap --script vuln 192.168.1.1`
- `OpenVAS`: An open source vulnerability scanner and manager.
  - Syntax: `openvas-cli -h <IP or hostname> -u <username> -w <password> -c "<command>"`
  - Example: `openvas-cli -h 192.168.1.1 -u admin -w admin -c "get_tasks"`
- `Nikto`: A web server scanner that checks for vulnerabilities such as SQL injection and cross-site scripting (XSS).
  - Syntax: `nikto -h <IP or hostname>`
  - Example: `nikto -h 192.168.1.1`
- `Arachni`: A modular web application security scanner that checks for SQL injection, cross-site scripting (XSS), and other vulnerabilities.
  - Syntax: `arachni <target>`
  - Example: `arachni http://example.com/`
- `Metasploit`: A penetration testing framework that includes tools for exploit development, post-exploitation, and social engineering.
  - Syntax: `msfconsole`
  - Example: `msfconsole`

## System Hacking

- `Hydra`: A network logon cracker that supports numerous services such as FTP, SMTP, and Telnet.
  - Syntax: `hydra -l <username> -P <password file> <IP or hostname> <service>`
  - Example: `hydra -l admin -P passwords.txt 192.168.1.1 ftp`
- `John the Ripper`: A password cracking tool that can be used to crack passwords on a variety of systems and platforms.
  - Syntax: `john --wordlist=<wordlist> <password file>`
  - Example: `john --wordlist=/usr/share/wordlists/rockyou.txt password.txt`
- `Medusa`: A network password cracking tool that supports numerous services such as FTP, SSH, and Telnet.
  - Syntax: `medusa -h <IP or hostname> -U <usernames file> -P <passwords file> -M <service>`
  - Example: `medusa -h 192.168.1.1 -U users.txt -P passwords.txt -M ssh`
- `Aircrack-ng`: A suite of tools for auditing wireless networks.
  - Syntax: `aircrack-ng <capture file>`
  - Example: `aircrack-ng capture.cap`

## Hacking Web Applications

- `Burp Suite`: A web application security testing tool that includes a web proxy, web spider, and other tools for testing web applications.
  - Syntax: `burpsuite`
  - Example: `burpsuite`
- `OWASP ZAP`: A web application security scanner that includes a proxy, scanner, and numerous other tools for testing web applications.
  - Syntax: `zap`
  - Example: `zap`
- `sqlmap`: A tool for automated SQL injection and database takeover.
  - Syntax: `sqlmap -u <URL>`
  - Example: `sqlmap -u http://example.com/vulnerable.php?id=1`
- `DirBuster`: A tool for discovering hidden directories and files on a web server.
  - Syntax: `dirbuster`
  - Example: `dirbuster`
