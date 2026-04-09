# CoreBank-Network

<img width="1769" height="781" alt="Screenshot 2026-04-09 140938" src="https://github.com/user-attachments/assets/e3e94c0e-b190-4479-9b20-064fcfd58c72" />

# 🏦 CoreBank-Network
### Enterprise Banking Network Infrastructure
**by Belal Eladawy**

---

## 📌 Project Overview

**CoreBank-Network** is a full enterprise banking network simulation built in **Cisco Packet Tracer**, designed to reflect a real-world bank's internal network infrastructure. The network separates departments using **VLANs**, ensures automatic IP distribution via **DHCP**, and uses a **Multilayer Switch (Cisco 3560)** as the core routing engine for inter-department communication — all while keeping each department isolated for maximum security.

---

## 🏢 Network Departments

| Department | Devices | VLAN | Network |
|---|---|---|---|
| 🩷 **Operations / Back Office** | PC0 – PC55 (56 PCs) | VLAN 10 | 192.168.10.0/24 |
| 🩵 **Management / Executive** | Laptop7 – Laptop17 + PCs | VLAN 20 | 192.168.20.0/24 |
| 💚 **IT / Technical Staff** | Laptop0 – Laptop6 | VLAN 30 | 192.168.30.0/24 |
| 🖥️ **Data Center** | Server0 – Server8 | VLAN 40 | 192.168.40.0/24 |

---

## 🔧 Technologies Used

| Technology | Role |
|---|---|
| **Cisco 3560 Multilayer Switch** | Core routing + inter-VLAN routing |
| **Cisco 2960-24TT Switches** | Department-level switching |
| **VLANs (10/20/30/40)** | Department isolation & security |
| **Inter-VLAN Routing (SVI)** | Communication between departments |
| **DHCP** | Automatic IP assignment per VLAN |
| **Trunk Links** | Carrying multiple VLANs between switches |
| **Access Ports** | Connecting end devices per department |

---

## 📋 IP Addressing Table

| Device | VLAN | IP Range | Gateway | DNS |
|---|---|---|---|---|
| PC0 – PC55 | 10 | 192.168.10.10 – .254 | 192.168.10.1 | 192.168.40.2 |
| Laptop7 – Laptop17 | 20 | 192.168.20.10 – .254 | 192.168.20.1 | 192.168.40.2 |
| Laptop0 – Laptop6 | 30 | 192.168.30.10 – .254 | 192.168.30.1 | 192.168.40.2 |
| Server0 – Server8 | 40 | 192.168.40.10 – .254 | 192.168.40.1 | 192.168.40.2 |

---

## 🚀 Future Enhancements

- [ ] Add Firewall between Data Center and all departments
- [ ] Implement ACLs — restrict Operations from sensitive servers
- [ ] Add DMZ for external-facing banking services
- [ ] Connect to **NetBridge** (BGP/OSPF) for multi-branch banking
- [ ] Add redundant uplinks (EtherChannel / HSRP)
- [ ] Implement QoS for priority banking traffic

---

## 👨‍💻 Author

**Belal Eladawy**
Network Engineer
