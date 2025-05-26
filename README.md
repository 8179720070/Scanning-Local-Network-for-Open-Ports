# Scanning-Local-Network-for-Open-Ports
First we have to install npcap for nmap scanning 
Nmap is used to scan the ip address
nmap shows the open and closed ports on the ip address 
In windows to know the ip address of our machine we have to open terminal and enter command "ipconfig"![IMG-20250526-WA0009](https://github.com/user-attachments/assets/bb85984d-ed7d-44c1-abe5-ed6a275c020b)
In Linux to know the ip address of our machine we have to open terminal and enter command "ifconfig"
After entering the command we get ip address of our machine 
Now open the nmap to scan the open and closed ports on  ip address
To perform tcp syn scan enter the Command - nmap -sS 192.168.51.117
![IMG-20250526-WA0000](https://github.com/user-attachments/assets/1011840b-aa6b-420a-b9ea-aae4e6f3d4c2)
After scanning we see that 4 ports are open and 996 ports are closed
services on the open ports![IMG-20250526-WA0010](https://github.com/user-attachments/assets/5d50f7f8-f2cf-45a0-8413-d6f7cf16a7aa)
# common services
# port 135 - Enables remote communication between clients and servers in Windows environments
# Port 139 - Printer and file-sharing services use port 139 to provide SMB over NetBIOS session services, which transmit large messages and other heavy traffic over a network between two devices over NetBIOS.
# Port 445 - TCP port 445 is used for direct TCP/IP MS Networking access without the need for a NetBIOS layer.
# Port 5432 - Port 5432 facilitates connections from PostgreSQL clients to PostgreSQL servers.
# potential security risks from open ports #
# Port 135 - It can be exploited by attackers to execute arbitrary code, gain unauthorized access to sensitive data or launch DDoS attacks.
# Port 139 - Exploit vulnerabilities in SMB services running on Port 139 to initiate attacks such as ransomware, data breaches, and espionage.
# Port 445 - TCP 445's open nature can also be its Achilles' heel, exposing networks to unauthorized access and malicious exploits.
# Port 5432 -  It can present several security risks like - Unauthorized Access,Exploitation of Vulnerabilities,Data Exfiltration,SQL Injection Amplification,Information Disclosure, Denial of Service (DoS), Weak or Missing Encryption
To save scan results we use command # nmap -oN output.txt nmap -oN output.txt 192.168.51.117
<content://media/external/file/1000088990>
