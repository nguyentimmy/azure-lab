# RDP Brute Force Lab

The purpose of this lab is to detect and alert brute forcing on machines that has RDP enabled. In this demonstration, I've performed a brute force attack using Hydra. 



***

# Session 1 

First step from an attacker perspective is to scan the subnet to see what devices or ports are available in the network.

- **Bullet 1:** As you can see on the result on the nmap scan, RDP is open on this Windows workstation/server. By default, RDP will be located on Port 3389. Ideally you shouldn't keep RDP open to the public facing internet. In this case since this machine is running on Azure, it's best set up a Bastion Host. A bastion host connects the VM on a browser without needing to RDP or SSH to VM. It eliminates exposing VM via on public IP. Also to an extent, it protects against port scanning. 

- **Bullet 2:** I performed a brute foce attacking using Hydra.

![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/1.%20rdp%20bf.png)

***


# Session 2

![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/2.%20rdp%20bf.png)

***


# Session 3

![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/3.%20rdp%20bf.png)

***

# Session 4

![alt text](https://github.com/nguyentimmy/azure-lab/blob/main/Azure%20Pen%20Testing/RDP%20Brute%20Force/Pictures/4.%20rdp%20bf.png)

***

