```bash
nmap -vv --reason -Pn -T4 --min-rate=1000 -sV -p 445 --script="banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN "/home/parallels/HacktheBox/OSCP-like/AD-Cascade/results/10.10.10.182/scans/tcp445/tcp_445_smb_nmap.txt" -oX "/home/parallels/HacktheBox/OSCP-like/AD-Cascade/results/10.10.10.182/scans/tcp445/xml/tcp_445_smb_nmap.xml" 10.10.10.182
```

[/home/parallels/HacktheBox/OSCP-like/AD-Cascade/results/10.10.10.182/scans/tcp445/tcp_445_smb_nmap.txt](file:///home/parallels/HacktheBox/OSCP-like/AD-Cascade/results/10.10.10.182/scans/tcp445/tcp_445_smb_nmap.txt):

```
# Nmap 7.93 scan initiated Fri Nov 18 15:56:55 2022 as: nmap -vv --reason -Pn -T4 --min-rate=1000 -sV -p 445 "--script=banner,(nbstat or smb* or ssl*) and not (brute or broadcast or dos or external or fuzzer)" -oN /home/parallels/HacktheBox/OSCP-like/AD-Cascade/results/10.10.10.182/scans/tcp445/tcp_445_smb_nmap.txt -oX /home/parallels/HacktheBox/OSCP-like/AD-Cascade/results/10.10.10.182/scans/tcp445/xml/tcp_445_smb_nmap.xml 10.10.10.182
Nmap scan report for 10.10.10.182
Host is up, received user-set (0.029s latency).
Scanned at 2022-11-18 15:57:03 AEDT for 42s

PORT    STATE SERVICE       REASON  VERSION
445/tcp open  microsoft-ds? syn-ack
|_smb-enum-services: ERROR: Script execution failed (use -d to debug)

Host script results:
| smb2-capabilities: 
|   202: 
|     Distributed File System
|   210: 
|     Distributed File System
|     Leasing
|_    Multi-credit operations
| smb-protocols: 
|   dialects: 
|     202
|_    210
| smb-mbenum: 
|_  ERROR: Failed to connect to browser service: Could not negotiate a connection:SMB: Failed to receive bytes: ERROR
| smb2-time: 
|   date: 2022-11-18T04:57:17
|_  start_date: 2022-11-18T04:53:54
|_smb-print-text: false
|_smb-vuln-ms10-061: Could not negotiate a connection:SMB: Failed to receive bytes: ERROR
| smb2-security-mode: 
|   210: 
|_    Message signing enabled and required

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Fri Nov 18 15:57:45 2022 -- 1 IP address (1 host up) scanned in 49.98 seconds

```
