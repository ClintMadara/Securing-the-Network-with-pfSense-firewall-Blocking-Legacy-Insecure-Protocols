<img width="405" height="449" alt="Screenshot 2026-05-03 160727" src="https://github.com/user-attachments/assets/74914fa1-7007-4355-bfed-ebc25513c072" /># Securing-the-Network-with-pfSense-firewall-Blocking-Legacy-Insecure-Protocols

This lab demonstrates how to harden a network using a pfSense firewall by blocking legacy and insecure protocols such as Telnet, FTP, and HTTP. 
The objective is to reduce the attack surface by preventing plaintext communication, limiting lateral movement, and mitigating common exploitation techniques used by attackers.

🌐**Environment:**  
*VMware  
*pfSense  
*Windows 10, Windows server & Ubuntu  ISOs

<img width="584" height="751" alt="Untitled Diagram(4)" src="https://github.com/user-attachments/assets/d25b034f-0cc8-411e-8f0b-80f654066008" />

**Configuration Steps**  
I first downloaded the pfsense ISO and created a VM for the pfSense appliance, during the setup phase, I added two NICs to the firewall 
<img width="700" height="289" alt="image" src="https://github.com/user-attachments/assets/46115570-6f82-48aa-ae07-3561db85030b" />


I then configured WAN & LAN interfaces in VMware

One network interface is for the private network and the other network interface  is for the public network. This is to make sure that alll traffic goes through pfSense beofre leaving the local network.

<img width="291" height="40" alt="Screenshot 2026-05-03 155133" src="https://github.com/user-attachments/assets/c73e7b0e-c058-4ab6-8537-a3a3f4511067" />  

*I then assigned static IPs to the two NICs on the firewall  
*The two IPs are on 24 bit subnets but different networks

<img width="468" height="49" alt="Screenshot 2026-05-03 160020" src="https://github.com/user-attachments/assets/d42c8c33-b658-4988-9716-16ded08eea65" />

I then assigned static IP addresses to the Domain controller and other VMs in the network.  
Made sure that that pfsense is the default gateway for all machines in the network settings
<img width="405" height="449" alt="Screenshot 2026-05-03 160727" src="https://github.com/user-attachments/assets/4c49ac56-6a13-415f-b50d-8543ee220199" />  



