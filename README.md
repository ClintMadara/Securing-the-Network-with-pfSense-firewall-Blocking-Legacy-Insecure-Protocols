# Securing-the-Network-with-pfSense-firewall-Blocking-Legacy-Insecure-Protocols

This lab demonstrates how to harden a network using a pfSense firewall by blocking legacy and insecure protocols such as Telnet, FTP, and HTTP. 
The objective is to reduce the attack surface by preventing plaintext communication, limiting lateral movement, and mitigating common exploitation techniques used by attackers.

🌐**Environment:**  
*VMware  
*pfSense  
*Windows 10, Windows server & Ubuntu  ISOs

<img width="584" height="751" alt="Untitled Diagram(4)" src="https://github.com/user-attachments/assets/d25b034f-0cc8-411e-8f0b-80f654066008" />

**Configuration Steps**  
I first downloaded the pfsense ISO and created a VM for the pfSense appliance, during the setup phase, I added two NICs to the firewall  

I then configured WAN & LAN interfaces in VMware

One network interface is for the private network and the other network interface  is for the public network

<img width="291" height="40" alt="Screenshot 2026-05-03 155133" src="https://github.com/user-attachments/assets/44250aab-f8f4-45b0-bf4a-d6f110d9282f" />

