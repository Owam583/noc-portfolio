# noc-portfolio
NOC Intern portfolio showcasing CCNA labs, network monitoring concepts, troubleshooting workflows, and exposure to ticketing systems and monitoring tools used in day-to-day NOC operations.

Taking the initiative to strengthen my technical skills through hands-on networking practice using **MikroTik Cloud Hosted Router (CHR) on VirtualBox** ~ _Building my networking skills one configuration at a time._

**MIKROTIK CHR INSTALLATION AND ROUTER CONFIGURATION IN VIRTUALBOX**

CHAPTER 1 - BASIC CONFIGURATIONS

01 - Identity: I successfully configured my router hostname as CHR_router_one
command: _system identity set name=CHR_router_one_
verification: _system identity print_

<img width="525" height="53" alt="image" src="https://github.com/user-attachments/assets/23c502e4-a894-4061-99a2-25e1b5ab8e8b" />

02 - Interface enabling & naming
Devices within a network communicate through physical or logical network interfaces. On my MikroTik CHR, we have two network interfaces: `ether1` and `ether2`. For easier identification and network management, we will rename `ether1` to **WAN** and `ether2` to **LAN**.
command: interface set <int-id> name=<int-name>
<img width="500" height="18" alt="image" src="https://github.com/user-attachments/assets/2a54a3b6-15be-4340-a201-dc1b55e06082" />
<img width="496" height="21" alt="image" src="https://github.com/user-attachments/assets/f1fa761a-3532-49bb-bc38-b62a92ac52b3" />
<img width="475" height="102" alt="image" src="https://github.com/user-attachments/assets/d6b0adb9-f19c-46b8-9743-83b3f8164e16" />

03 - IP Addressing
Every device on an IP-based network requires an IP address for communication. My MikroTik `ether1` (WAN) receives its IP address automatically through DHCP.
<img width="482" height="85" alt="image" src="https://github.com/user-attachments/assets/aa0ee238-5840-4792-a504-e2b786a5c0b3" />

For the manually configured interface, `ether2` (LAN), we will assign a static IP address to enable communication between devices on the local network.
command: ip address add address=x.x.x.x/xx interface=<port-id>
 <img width="703" height="24" alt="image" src="https://github.com/user-attachments/assets/c9a2af0e-60c1-4622-aec1-f11ad8dba151" />
verify: <img width="484" height="101" alt="image" src="https://github.com/user-attachments/assets/d64709db-c1ee-40a2-a636-e42375d986ec" />




