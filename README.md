# 🏨 Hotel Network System – CCNA Final Project

## 📌 Overview

A fully segmented and scalable hotel network infrastructure created using **Cisco Packet Tracer** as part of the CCNA final project at NTI. The system simulates real-world enterprise networking across 3 floors, each containing specific departments. The project includes VLANs, inter-VLAN routing, DHCP, subnetting, and OSPF dynamic routing.

---

## 🔑 Key Features

- 🧱 **VLAN Segmentation**  
  Logical separation of departments using VLANs to enhance security and broadcast efficiency.

- 🔀 **Router-on-a-Stick**  
  Inter-VLAN communication via sub-interfaces configured on a single router interface.

- 🎯 **DHCP Server Integration**  
  Dynamic IP assignment for each VLAN through centralized DHCP pools.

- 🛰 **OSPF Dynamic Routing**  
  Routers exchange routes and build dynamic routing tables over serial point-to-point links.

- 🧮 **Custom Subnetting Plan**  
  Efficient address usage using subnetted Class A (`10.10.10.0/8`) for WAN links.

- 📶 **Layer 2 Switching**  
  Switches configured with trunk and access ports for proper VLAN tagging and traffic flow.

---

## 🏢 Floor Structure

| Floor | Departments | VLAN ID | Subnet             |
|-------|-------------|---------|--------------------|
| 1     | Reception   | 10      | 192.168.10.0/24    |
|       | Store       | 20      | 192.168.20.0/24    |
|       | Logistics   | 30      | 192.168.30.0/24    |
| 2     | Finance     | 40      | 192.168.40.0/24    |
|       | HR          | 50      | 192.168.50.0/24    |
|       | Sales       | 60      | 192.168.60.0/24    |
| 3     | Admin       | 70      | 192.168.70.0/24    |
|       | IT          | 80      | 192.168.80.0/24    |

---

## ⚙️ Technologies Used

- Cisco Packet Tracer  
- Router-on-a-Stick  
- OSPF Routing Protocol  
- DHCP Services  
- Custom Subnetting  
- Layer 2 Switching

---

## 🔗 IP & Subnetting Plan

### 📡 WAN Links (Point-to-Point - /30 Subnets)

| Link | Network         | Host 1        | Host 2         | Broadcast       |
|------|-----------------|---------------|----------------|-----------------|
| n1   | 10.10.10.0/30   | 10.10.10.1    | 10.10.10.2     | 10.10.10.3      |
| n2   | 10.10.10.4/30   | 10.10.10.5    | 10.10.10.6     | 10.10.10.7      |
| n3   | 10.10.10.8/30   | 10.10.10.9    | 10.10.10.10    | 10.10.10.11     |

### 🖧 LAN Subnets

Each VLAN is assigned a full Class C subnet (/24), with DHCP handling host IP allocation.

---

## 🚀 How to Run

1. Open the `.pkt` file in **Cisco Packet Tracer**.  
2. Check VLAN and trunk configurations on switches.  
3. Verify sub-interfaces and DHCP pools on the router.  
4. Run `ping` tests across departments to verify routing.  
5. Use `show vlan`, `show ip route`, and `show ip ospf neighbor` for verification.

---

## 📷 Demo

- **Topology Screenshot**
- [![image.png](https://i.postimg.cc/B6dcNjC1/image.png)](https://postimg.cc/ftf9RTpw)
- **Subnetting Plan Image**  
-[![Screenshot-2025-09-19-184323.png](https://i.postimg.cc/dV7fWFqd/Screenshot-2025-09-19-184323.png)](https://postimg.cc/zyrpB9HX)

---


## 👨‍🎓 Author

**Name:** [ZiadRehan]  
**Institute:** National Telecommunication Institute (NTI)  
**Course:** CCNA Final Project  
**Date:** September 2025

---

## 📝 File List

| File                 | Description                    |
|----------------------|-------------------------------|
| [`HotelNetwork.pkt`](./HotelNetwork.pkt)    | Main Cisco Packet Tracer project |
| [`README.md`](./README.md)          | This documentation             |
| [`Documentation.pdf`](./Documentation.pdf) | Full technical report          |
| [`subnet-plan.png`](./subnet-plan.png)    | Subnetting and IP planning     |
| [`topology.png`](./topology.png)       | Network diagram screenshot     |





<p align="right">
  <img src="https://i.postimg.cc/yxy6x7F6/image.png" width="32" valign="middle">
  <a href="mailto:zezorehan938@gmail.com" style="font-weight:bold; font-size:20px; text-decoration:underline; color:#2e89ff;">
    𝓩𝓲𝓪𝓭𝓻𝓮𝓱𝓪𝓪𝓷
  </a>
</p>
