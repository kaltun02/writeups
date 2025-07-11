# HTB - Dancing
IP Address: (10.10.171.186)
Difficulty: Easy
Category: Enumeration / SMB

Tools Used:
nmap 

Steps to Exploit:
  Service Scan
Ran an nmap scan to discover open ports and services:
nmap -sC -sV -Pn <IP>

Found SMB running on port 445

SMB Enumeration:
Used the scan results to explore SMB shares and identify accessible files.

Flag Retrieval
Accessed the available SMB share, navigated through the directories, and found the user flag

Notes:
This box focused on basic SMB enumeration.

Great practice for learning how file shares can expose sensitive info if misconfigured.
