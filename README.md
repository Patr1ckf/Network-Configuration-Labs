# GNS3 Network Configuration Labs

## Project Overview
This repository contains configuration files and reports from four networking labs conducted in GNS3, focusing on various network configuration techniques. These labs provide hands-on experience in network design, routing protocols, and network address translation (NAT), covering both static and dynamic routing as well as VLAN implementation. The key areas explored include:

1. **Static Routing** – Manual route configuration between routers
2. **Dynamic Routing** – Automated route learning using RIP v2, OSPF, and BGP
3. **NAT (Network Address Translation)** – IP address translation for external connectivity
4. **VLAN (Virtual Local Area Network)** – Network segmentation using VLANs

Each lab includes detailed configurations, testing procedures, and verification steps, ensuring practical understanding of networking principles.

## Repository Contents
The repository includes configurations for the four networking labs:

1. **Static Routing** – Implementation of manually defined routes between routers.
2. **Dynamic Routing** – Configuration of RIP v2, OSPF, and BGP to enable automatic routing.
3. **NAT** – Applying NAT techniques to allow communication between private and public networks.
4. **VLAN** – Setting up VLANs to segment network traffic efficiently.

## Detailed Lab Descriptions

### 1. Static Routing
- **Objective**: Configure static routing between network devices.
- **Tools Used**: GNS3, routers, switches, virtual machines.
- **Configuration Steps**:
  - Define IP addressing scheme and subnetting.
  - Assign static routes on routers using `ip route` commands.
  - Verify connectivity using `ping` and `show ip route`.
- **Key Concepts**: IP addressing, subnetting, static routing, inter-subnet communication.

### 2. Dynamic Routing
- **Objective**: Implement dynamic routing protocols to ensure end-to-end connectivity.
- **Protocols Covered**:
  - **RIP v2**: Distance-vector routing protocol with hop count as metric.
  - **OSPF**: Link-state routing protocol using Dijkstra’s algorithm.
  - **BGP**: Border Gateway Protocol for inter-AS routing.
- **Configuration Steps**:
  - Enable RIP v2, OSPF, and BGP on respective routers.
  - Define network statements and establish neighbor relationships.
  - Configure route redistribution for cross-protocol communication.
- **Verification**:
  - Check routing tables (`show ip route`), Wireshark packet captures.
  - Test connectivity using `ping` and `traceroute`.

### 3. NAT (Network Address Translation)
- **Objective**: Enable private-to-public IP translation for network access.
- **Configuration Steps**:
  - Define NAT pool and access lists for address translation.
  - Apply NAT rules on router interfaces (`ip nat inside` and `ip nat outside`).
  - Enable overloading for PAT (Port Address Translation).
- **Verification**:
  - Use `show ip nat translations` to check address mappings.
  - Conduct `ping` tests to confirm successful translation.

### 4. VLAN (Virtual Local Area Network)
- **Objective**: Implement VLANs for network segmentation and isolation.
- **Configuration Steps**:
  - Create VLANs and assign ports to VLANs.
  - Configure trunking between switches (`switchport mode trunk`).
  - Enable inter-VLAN routing using a Layer 3 switch or router-on-a-stick.
- **Verification**:
  - Check VLAN assignment (`show vlan brief`).
  - Test communication between VLANs.

