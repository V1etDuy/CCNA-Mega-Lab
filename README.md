# 🌐 Enterprise Network Design & Implementation | CCNA Mega Lab

![Cisco Packet Tracer](https://img.shields.io/badge/Simulator-Cisco%20Packet%20Tracer-005A70?style=for-the-badge&logo=cisco&logoColor=white)
![Network](https://img.shields.io/badge/Protocols-OSPF%20|%20HSRP%20|%20LACP-blue?style=for-the-badge)
![Security](https://img.shields.io/badge/Security-ACL%20|%20DHCP%20Snooping-red?style=for-the-badge)

## 📖 Overview
This project demonstrates a comprehensive, end-to-end configuration of a high-availability enterprise network. It covers the full spectrum of the **Cisco CCNA 200-301** curriculum, transitioning from basic initial setup to complex multi-layer switching, dynamic routing, and wireless infrastructure management.

> **Status:** 100% Completed (Verified by Packet Tracer Activity Grading)

---

## 🏗️ Topology & Architecture
The network is structured using a hierarchical design (Core - Distribution - Access) across two main offices (Office A & Office B), featuring:
- **Redundant Internet Edge:** Dual ISP connections via R1.
- **EtherChannel Trunking:** Link aggregation for high-bandwidth uplinks.
- **L3 Core:** High-speed routing at the core layer.

---

## 🛠️ Key Technologies Implemented

### 1. Switching (Layer 2)
- **VLANs & VTP:** Logical segmentation for PCs, Phones, WiFi, and Management.
- **Spanning Tree (Rapid PVST+):** Loop prevention with root bridge optimization to align with HSRP.
- **EtherChannel:** Implementation of both **LACP** (Open Standard) and **PAgP** (Cisco Proprietary).

### 2. Routing (Layer 3)
- **OSPFv2 (Multi-area):** Dynamic routing with Point-to-Point network types and passive interfaces.
- **HSRP (Hot Standby Router Protocol):** Default gateway redundancy for end-user subnets.
- **IPv4/IPv6:** Dual-stack implementation including Static and Floating Static routes.

### 3. Network Services & Security
- **DHCP Server & Relay:** Automated IP addressing with R1 acting as the central server.
- **NAT/PAT:** Static NAT for Server 1 and Dynamic PAT for LAN-to-Internet traffic.
- **Hardening:** Implementation of Port Security, DHCP Snooping, Dynamic ARP Inspection (DAI), and SSHv2.
- **Infrastructure:** NTP Synchronization, SNMP Read-Only, and Syslog logging.

### 4. Wireless Infrastructure
- **WLC Configuration:** Centralized management of Lightweight Access Points (LWAPs).
- **Security:** WPA2-AES encryption for Wireless LANs.

---

## 🚀 Lab Highlights
* **Recursive & Fully Specified Routing:** Configured sophisticated routing paths for failover testing.
* **Infrastructure Management:** Performed an **IOS Upgrade** via FTP on R1 to simulate real-world maintenance.
* **Security Best Practices:** Disabled unused ports, implemented BPDU Guard, and restricted SSH access via Standard ACLs.

---

## 📂 Project Structure
```text
├── Topology_Snapshot.png    # High-resolution image of the network
├── Configs/                 # Device-specific running configs (.txt)
│   ├── R1_Router.txt
│   ├── Core_Switch_1.txt
│   └── Dist_Switch_A1.txt
└── README.md                # Project documentation

---
```
## 👤 Contact Information

**Duy Viet** *Network Engineering Enthusiast*
* **Lab Credit:** Based on the *Jeremy's IT Lab* CCNA curriculum.
