Project Title: Local Network Open Port Scan
Objective: The objective of this project is to learn how to discover open ports on devices in a local network in order to understand network exposure and potential security risks.
Tool Used: Nmap – For scanning the local network to find devices and open ports.

Wireshark (optional) – For capturing and analyzing network traffic.
Steps Performed: 1. Installed Nmap from the official website on my Windows PC.
2. Identified local IP and network range using ipconfig. My IP was ------- with subnet mask 255.255.255.0, so the network range was 192.168.116.0/24.
Ran a TCP SYN scan using Nmap: nmap -sS 192.168.116.0/24
Researched services running on the open ports and identified potential security risks.

Saved scan results in a text file (Local;NetworkScan) in the project folder for documentation.
FINDING

| IP Address     | Open Ports  | Service          | Potential Risk                                               |
| 192.168.116.61 |  53           Domain              DNS Amplification Attacks , DNS cache Poisoning
| 192.168.116.90 | 135         |  msrpc           |unauthorized access or malicious code execution.

                   139         |netbios-ssn       |unauthorized access to sensitive information or network disruption.

                   495         |microsoft-ds      |difficult to determine without knowing the specific service, but potentially exploitable.

                   7070        |realserver        |unauthorized access to sensitive information or disruption of streaming services.
5. Port 8080: HTTP Proxy/Web Server - Potential risk: unauthorized access to sensitive information, malware injection, or web service disruption  of streaming services.



                   8080        |opsmessaging      |unauthorized access to sensitive information, malware injection, or web service disruption.


                   
Conclusion:

Through this project, I learned how to scan a local network to discover devices and open ports. I understood which ports are commonly used by services and the potential security risks associated with leaving ports open. This project helped me gain practical experience in network scanning, documentation, and understanding network exposure, which is an important aspect of cybersecurity.            