# Enterprise Office Network Design – Cisco Packet Tracer

## 🎓 Academic Project Information
**Degree:** BSc (Hons) Computer Networks  
**Module:** Advanced Networking (CIS005-3)  
**University:** University of Bedfordshire  

**Student:** V. Gurunivasan  
**Student ID:** 2526303  
**Instructor:** Mr. Vibhavi Attigala  

**Assignment Type:** Individual Coursework – Network Design & Implementation

---

## 🏢 Project Background
This repository contains a comprehensive **enterprise network design and implementation** for **Crescent Studios**, a creative animation and production company.  

The project was developed as part of the *Advanced Networking (CIS005-3)* module and demonstrates the **practical application of real-world enterprise networking concepts** within a simulated production environment using **Cisco Packet Tracer**.

The design focuses on:
- Departmental network segmentation
- Secure inter-department communication
- Scalable architecture
- Controlled access using ACLs
- Centralized IP management

---

## 📌 Project Overview
This project presents the design and implementation of a **secure, scalable enterprise office network** using Cisco Packet Tracer. The network follows **industry-aligned enterprise design principles**, including VLAN segmentation, inter-VLAN routing, centralized DHCP, and access control using ACLs.

The objective of this project is to simulate a realistic office environment with multiple departments, secure internal communication, controlled inter-department access, and safe internet connectivity.

---

## 🏢 Network Design Approach
The network is designed using a **hierarchical architecture**:

- **Core Layer** – Layer 3 switch responsible for inter-VLAN routing
- **Distribution Layer** – Departmental routing and policy enforcement
- **Access Layer** – End-user connectivity (wired and wireless)

This structure improves scalability, performance, fault isolation, and security.

---

## 🌐 VLAN Architecture
Each department is assigned a dedicated VLAN and subnet to ensure **network segmentation and security**.

| VLAN ID | VLAN Name            | Subnet            | Purpose |
|-------|---------------------|-------------------|--------|
| 10    | Tech-Staff          | 192.168.1.0/24    | Technical staff devices |
| 20    | Tech-Members        | 192.168.2.0/24    | Technical department members |
| 30    | Tech-Guests         | 192.168.3.0/24    | Guest users (technical area) |
| 40    | Ops-Staff           | 192.168.4.0/24    | Operations staff |
| 50    | Ops-Members         | 192.168.5.0/24    | Operations department members |
| 60    | Ops-Guests          | 192.168.6.0/24    | Guest users (operations area) |
| 99    | Management          | 192.168.99.0/24   | Network management |

---

## 🔐 Access Control (ACL) Summary
Access Control Lists (ACLs) are used to enforce **departmental security policies**.

- Staff VLANs can access their respective department resources
- Cross-department access is restricted unless explicitly required
- Guest VLANs are isolated from all internal networks
- All VLANs are permitted controlled internet access

This approach reduces the risk of unauthorized access and lateral movement.

---

## 📡 Wireless Network Design
The wireless network is segmented using multiple SSIDs mapped to VLANs:

- **Staff SSID** → Staff VLANs
- **Members SSID** → Members VLANs
- **Guest SSID** → Guest VLANs (Internet-only access)

Wireless users are subject to the same ACL and security policies as wired users.

---

## 📦 DHCP Configuration
IP address assignment is handled using **centralized DHCP**, allowing:

- Automatic IP allocation
- Reduced manual configuration
- Simplified network administration
- Consistent addressing across VLANs

Each VLAN is assigned a dedicated DHCP pool.

---

## 🧪 Testing & Validation
The network was tested for:
- Inter-VLAN communication
- ACL enforcement
- DHCP address assignment
- Internet connectivity
- Wireless isolation

All test cases were validated successfully in Cisco Packet Tracer.

---

## 🛠 Tools Used
- Cisco Packet Tracer
- Cisco IOS (Switching & Routing)
- VLANs, SVIs, DHCP, ACLs
- Wired and Wireless Enterprise Networking Concepts

---

## 📁 Repository Contents
- `SA2526303.pkt` – Cisco Packet Tracer simulation file
- `SA2526303.pdf` – Detailed design and evaluation report

---

## 📚 Author
Designed and implemented as part of an academic networking assignment by V. Gurunivasan.

---

## ⚠️ Disclaimer
This project is intended for **educational purposes** and network design demonstration only. All companies that are potrayed in the project are merely fictional.
