# Designing_a_secure_network
Your company faces an exciting challenge: designing a secure and efficient network for a client relocating to a new office. Their current setup requires modernization, and you're tasked with crafting a cost-effective, well-structured plan that optimizes resource allocation while adhering to stringent security best practices.

Constraints and Requirements:

Firewall Simulation: While Packet Tracer may not fully support advanced firewall configuration, we'll implement alternative security measures (explained later).

Client Requirements:

Active Directory and DNS server
DHCP server
DMZ concept implemented through VLANs and access control lists (ACLs) (firewall alternative)
iSCSI storage server
Four network sectors:

Management/Secretariat (5 workstations)

Study (8 workstations)

Production (10 workstations)

Support (2 sectors, 10 workstations each)

1. Diagram
<img width="313" alt="image" src="https://github.com/Lieul000/Designing_a_secure_network/assets/155724755/a4643f6d-89ac-4f24-b9ae-91d700c0c167">

2.	IP addressing table and VLAN

<img width="656" alt="Capture d’écran 2024-04-05 à 11 15 45" src="https://github.com/Lieul000/Designing_a_secure_network/assets/155724755/ab968940-79f6-410f-99a0-8b26f0a7e7af">


3.	KEY devices

Routers to create the LAN and to have access to WAN
Servers to connect all company’s department and host (such as printers and phone for example)
Switches and multilayer switch for the LAN and to assure the possibility to grow in the future and add some more departments.

4.	Security measures

TREE Topology 
+ cost efficient, scalability, flexibility, reliability, and security 
-higher cost and complexity

DMZ   to isolate traffic using : VLANS and ACLS to simulate firewall in packet tracer
-	Containing 3 separate servers(storage, DNS/AD Directory and DHCP)
-	VLANS (trunks)
-	ACLS to protect server from the outside network







5.	Cost breakdown of network components

2 routers 911 = 2 x 850€ soit 1700€
3 servers CISCO = 3 x 2000€ soit 6000€
1 Switch 2960-24TT = & x 1500 soit 1500 €
4 switchs 2950T-24 = 4 x 550€ soit 2200€
1 switch 3560-24PS layer 3 = 1500€
33 computers = 33 x 1000€ soit 33 000 €

+ Various cables ethernet  soit 300 €

TOTAL AMOUNT = 38500 €
![image](https://github.com/Lieul000/Designing_a_secure_network/assets/155724755/cbda59ad-57ab-4409-b8cb-ccf1f199e9fa)

