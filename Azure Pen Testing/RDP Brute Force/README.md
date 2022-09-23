# RDP Brute Force Lab

The purpose of this lab is to detect and alert brute forcing on machines that has RDP enabled. In this demonstration, I've performed a brute force attack using Hydra. I will provide POC that includes commands, syntax, and screenshots. 



***

# Session 1 

First step from an attacker perspective is to scan the subnet to see what devices or ports are available in the network.


- **Bullet 1:** As you can see on the result on the nmap scan, RDP is open on this Windows workstation/server. Depending on the scenario, it's best not to use these NMAP flags. This scan is very loud and can get detected by most modern security solutions (EX: IDS, IPS, SIEM, EDR, XDR). But for the sake of demonstration purposes, I will run the scans anyway.
  ```
  nmap -sC -sV -vvv -T5 -oN report.txt 10.0.0.4
  ```

- **Bullet 2:** I performed a brute force attacking using Hydra.
   ```
   hydra -t 1 -V -l winserver -P rockyou.txt rdp://10.0.0.4
   ```
   
![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/1.%20rdp%20bf.png)

***


# Session 2

First step from an attacker perspective is to scan the subnet to see what devices or ports are available in the network.

- **Bullet 1:** 
- **Bullet 2:** 

![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/2.%20rdp%20bf.png)

***


# Session 3

![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/3.%20rdp%20bf.png)

***

# Session 4

![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/4.%20rdp%20bf.png)

***

