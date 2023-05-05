
## Footprinting and Reconnaissance

- `whois`: Queries the WHOIS database to find information about domain name registration.
  - Syntax: `whois <domain>`
  - Example: `whois google.com`
- `dnsenum`: Gathers information about a target's DNS, such as the IP addresses of DNS servers, mail servers, and other hosts associated with the domain.
  - Syntax: `dnsenum <domain>`
  - Example: `dnsenum example.com`
- `theharvester`: Gathers emails, subdomains, hosts, employee names, open ports and banners from different public sources.
  - Syntax: `theharvester -d <domain> -b <search engine>`
  - Example: `theharvester -d microsoft.com -b google`
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
- `Arachni`: A modular web application security scanner that checks for SQL injection, cross-site scripting (XSS), and
