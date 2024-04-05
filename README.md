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

GROUPS	VLAN ID	NETWORK ADDRESS	FIRST IP ADDRESS AV.	LAST IP ADDRESS AV.	DEFAULT 
GATEWAY
MANAGEMENT	192.168.3.0/28
VLAN 10
(14 Ip AV)	192.168.3.0/28	192.168.3.1	192.168.3.14	192.168.3.15
STUDY 	192.168.4.0/27
VLAN 20 (30 Ip AV)	192.168.4.0/27	192.168.4.1	192.168.10.30	192.168.0.31
PRODUCTION 1	192.168.5.0/26
VLAN 30 (62 Ip AV)	192.168.5.0/26	192.168.5.1	192.168.5.62	192.168.5.63
PRODUCTION 2	192.168.5.0/26
VLAN 30	192.168.5.0/26	192.168.5.1	192.168.5.62	192.168.5.63
ROUTEURS	192.169.1.0/30
(4 Ip AV)	192.168.1.0/30	192.168.1.1	192.186.1.2	192.168.1.3

SERVICE	IP ADDRESS
DHCP 	192.168.1.3/28
ACTIVE DIRECTORY/DNS	192.168.1.4/28
ISCSI STORAGE/RADIUS	192.168.1.5/28


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

