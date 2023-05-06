1. Scan a single target:
   ```
   nmap <target>
   ```

2. Scan multiple targets:
   ```
   nmap <target1> <target2> <target3>
   ```

3. Scan a range of hosts:
   ```
   nmap <start-ip> - <end-ip>
   ```

4. Scan an entire subnet:
   ```
   nmap <subnet>
   ```

5. Scan for open ports:
   ```
   nmap -p <port-range> <target>
   ```

6. Scan all ports:
   ```
   nmap -p- <target>
   ```

7. Scan for a specific service/version:
   ```
   nmap -sV -p <port> <target>
   ```

8. Scan for OS fingerprinting:
   ```
   nmap -O <target>
   ```

9. Scan using TCP SYN stealth:
   ```
   nmap -sS <target>
   ```

10. Scan using UDP:
    ```
    nmap -sU <target>
    ```

11. Scan using ICMP ping:
    ```
    nmap -PE <target>
    ```

12. Scan using TCP ping:
    ```
    nmap -PS <target>
    ```

13. Save output to a file:
    ```
    nmap -oN <output-file> <target>
    ```

E.g.

1. Scan a single target:
   ```
   nmap 192.168.1.1
   ```

2. Scan multiple targets:
   ```
   nmap 192.168.1.1 192.168.1.2 192.168.1.3
   ```

3. Scan a range of hosts:
   ```
   nmap 192.168.1.1-10
   ```

4. Scan an entire subnet:
   ```
   nmap 192.168.1.0/24
   ```

5. Scan for open ports:
   ```
   nmap -p 80,443 192.168.1.1
   ```

6. Scan all ports:
   ```
   nmap -p- 192.168.1.1
   ```

7. Scan for a specific service/version:
   ```
   nmap -sV -p 22 192.168.1.1
   ```

8. Scan for OS fingerprinting:
   ```
   nmap -O 192.168.1.1
   ```

9. Scan using TCP SYN stealth:
   ```
   nmap -sS 192.168.1.1
   ```

10. Scan using UDP:
    ```
    nmap -sU 192.168.1.1
    ```

11. Scan using ICMP ping:
    ```
    nmap -PE 192.168.1.1
    ```

12. Scan using TCP ping:
    ```
    nmap -PS 80,443 192.168.1.1
    ```

13. Save output to a file:
    ```
    nmap -oN output.txt 192.168.1.1
    ```
