# Enterprise Network Design & Simulation | Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates the design and simulation of an enterprise network using Cisco Packet Tracer.

The network was designed for three departments:

- Management
- HR
- IT

The project focuses on network segmentation, inter-VLAN communication, automatic IP addressing, switch security, and network troubleshooting.

## 🖥️ Network Architecture

The network consists of:

- 1 Cisco Router
- 2 Cisco Switches
- Multiple End Devices
- Three VLANs
- Router-on-a-Stick configuration
- DHCP services

## 🌐 VLAN & IP Addressing

| VLAN | Department | Network | Default Gateway |
|------|------------|---------|-----------------|
| 10 | Management | 192.168.10.0/24 | 192.168.10.1 |
| 20 | HR | 192.168.20.0/24 | 192.168.20.1 |
| 30 | IT | 192.168.30.0/24 | 192.168.30.1 |

## ⚙️ Technologies & Configurations

### VLAN Segmentation
Three VLANs were created to logically separate network traffic between departments.

### 802.1Q Trunking
Trunk links were configured between the network devices to carry traffic from multiple VLANs.

### Router-on-a-Stick
Inter-VLAN routing was implemented using router subinterfaces with 802.1Q encapsulation.

### DHCP
DHCP pools were configured for each VLAN to provide automatic IP address assignment to end devices.

### Port Security
Switch port security was implemented using:

- Sticky MAC addresses
- Maximum secure MAC address limit of 1
- Restrict violation mode

## 🧪 Testing & Verification

The network configuration was verified using Cisco IOS commands including:

- `show vlan brief`
- `show interfaces trunk`
- `show ip interface brief`
- `show ip dhcp pool`
- `show ip dhcp binding`
- `show port-security`
- `show interfaces status`

Connectivity was also tested using ICMP Ping between gateways and devices across different VLANs.

### Final Result

The final connectivity tests were successful with **0% packet loss** across the tested VLANs and gateways.

## 📂 Project File

The Cisco Packet Tracer project file is included in this repository:

`Enterprise_Network_Design_cisco.pkt`

## 🛠️ Technologies

- Cisco Packet Tracer
- Cisco IOS
- VLAN
- 802.1Q Trunking
- Router-on-a-Stick
- Inter-VLAN Routing
- DHCP
- Port Security
- Network Troubleshooting
  
## 🎯 Project Objective

The objective of this project was to gain practical experience in designing, configuring, securing, and troubleshooting a segmented enterprise network using Cisco networking technologies.

## 🎯 Project Objective

The objective of this project was to gain practical experience in designing, configuring, securing, and troubleshooting a segmented enterprise network using Cisco networking technologies.
