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
