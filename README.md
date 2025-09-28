# Hotel-Network-System
🏨 Hotel Network System – CCNA Final Project
📘 Overview

This project simulates a hotel’s internal network infrastructure, built using Cisco Packet Tracer as part of the final project for the CCNA course at NTI.
The network is designed with scalability, segmentation, and manageability in mind using:

VLANs

Router-on-a-Stick (Inter-VLAN Routing)

DHCP

OSPF Routing

Subnetting using Class A address space

🏢 Network Structure

The hotel consists of 3 floors, each with designated departments:

🔹 Floor 1:

Reception (VLAN 10 - 192.168.10.0/24)

Store (VLAN 20 - 192.168.20.0/24)

Logistics (VLAN 30 - 192.168.30.0/24)

🔹 Floor 2:

Finance (VLAN 40 - 192.168.40.0/24)

HR (VLAN 50 - 192.168.50.0/24)

Sales (VLAN 60 - 192.168.60.0/24)

🔹 Floor 3:

Admin (VLAN 70 - 192.168.70.0/24)

IT (VLAN 80 - 192.168.80.0/24)

⚙️ Features Implemented
✅ 1. VLAN Configuration

Departments are isolated into VLANs to enhance security and reduce broadcast domains.

✅ 2. Inter-VLAN Routing

Implemented using Router-on-a-Stick via sub-interfaces on the router (Gig0/0).

✅ 3. DHCP Server

The main router dynamically assigns IP addresses to devices in each VLAN.

✅ 4. OSPF Routing

All routers are connected via point-to-point serial links and run OSPF (single-area, area 0).

✅ 5. Subnetting

Used Class A address 10.10.10.0/8 and subnetted into /30 networks for serial links:

Link	Network	Host 1	Host 2	Broadcast
n1	10.10.10.0/30	10.10.10.1	10.10.10.2	10.10.10.3
n2	10.10.10.4/30	10.10.10.5	10.10.10.6	10.10.10.7
n3	10.10.10.8/30	10.10.10.9	10.10.10.10	10.10.10.11
🧪 Testing & Verification

Devices across VLANs can communicate via the router.

ping tested between different floors and departments.

Routing tables verified using show ip route.

OSPF neighbor adjacency confirmed with show ip ospf neighbor.

📁 Files Included

HotelNetwork.pkt – Cisco Packet Tracer project file

README.md – Project documentation

Documentation.pdf (optional) – Full detailed explanation

Screenshots of network topology and IP plans

👨‍💻 Author

Name: [Your Name]
Institute: National Telecommunication Institute (NTI)
Course: CCNA Final Project
Date: Sept 2025
