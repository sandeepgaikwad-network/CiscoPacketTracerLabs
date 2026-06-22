# Cisco Packet Tracer Labs

## 📘 Overview
This repository contains a collection of networking labs created using **Cisco Packet Tracer**.  
The labs cover fundamental and advanced topics in computer networking, including IPv4/IPv6 configuration, routing protocols, VLANs, WAN setup, and network security.  

The goal of this repo is to serve as a **learning portfolio** and a reference for anyone practicing networking concepts.

---

## 📂 Repository Structure

- `IPv4/` → Labs on IPv4 addressing and configuration  
  - Lab01_IPv4_Basic_Config.pkt  
  - Lab03_Router_Initial_Config_IPv4.pkt  
  - Lab08_Static_Routing_IPv4.pkt  
  - Lab10_RIP_IPv4.pkt  
  - Lab12_OSPF_IPv4.pkt  
  - Lab13_OSPF_MultiArea_IPv4.pkt  
  - Lab15_EIGRP_IPv4.pkt  

- `IPv6/` → Labs on IPv6 addressing and configuration  
  - Lab02_IPv6_Basic_Config.pkt  
  - Lab04_Router_Initial_Config_IPv6.pkt  
  - Lab09_Static_Routing_IPv6.pkt  
  - Lab11_RIPng_IPv6.pkt  
  - Lab14_OSPFv3_IPv6.pkt  
  - Lab16_EIGRPv6_IPv6.pkt  
  - Lab30_ACL_IPv6.pkt  

- `Routing/` → Labs on RIP, OSPF, EIGRP, GRE, BGP, Default Routing  
  - Lab31_Default_Routing.pkt  
  - Lab34_GRE_Tunneling.pkt  
  - Lab46_BGP_Routing.pkt  

- `Switching/` → Labs on VLANs, trunking, STP, EtherChannel, inter‑VLAN routing  
  - Lab17_Switch_Initial_Config.pkt  
  - Lab18_VLANs.pkt  
  - Lab19_DTP.pkt  
  - Lab20_VTP.pkt  
  - Lab21_Router_on_a_Stick.pkt  
  - Lab22_STP.pkt  
  - Lab23_PortFast_BPDU_Guard.pkt  
  - Lab24_EtherChannel.pkt  

- `Security/` → Labs on router security, ACLs, port security, password recovery  
  - Lab05_Basic_Router_Security.pkt  
  - Lab25_Port_Security.pkt  
  - Lab26_Standard_ACL_IPv4.pkt  
  - Lab27_Standard_ACL_IPv4.pkt  
  - Lab28_Extended_ACL_IPv4.pkt  
  - Lab29_Extended_ACL_IPv4.pkt  
  - Lab37_Advanced_Router_Security.pkt  
  - Lab42_Password_Recovery.pkt  

- `WAN/` → Labs on WAN setup, PPP authentication  
  - Lab06_WAN_Serial_Config.pkt  
  - Lab07_WAN_Ethernet_Config.pkt  
  - Lab45_PPP_Authentication.pkt  

- `NAT/` → Labs on NAT and PAT  
  - Lab32_Static_NAT.pkt  
  - Lab33_PAT.pkt  

- `Services/` → Labs on DHCP, Syslog, NTP, CDP  
  - Lab36_CDP.pkt  
  - Lab38_DHCP_Server_Client.pkt  
  - Lab39_Syslog.pkt  
  - Lab40_NTP.pkt  

- `IOS_Backup/` → Labs on IOS backup and licensing  
  - Lab43_IOS_Config_Backup.pkt  
  - Lab44_IOS_Licensing.pkt  


---

## 🧪 Lab Index

| Lab No. | Title | Description |
|---------|-------|-------------|
| 1 | [IPv4 Basic Config](IPv4/Lab01_IPv4_Basic_Config.pkt) | Configure IP addresses and test connectivity |
| 2 | [IPv6 Basic Config](IPv6/Lab02_IPv6_Basic_Config.pkt) | Set up IPv6 addressing and ping tests |
| 3 | [Router Initial Config (IPv4)](IPv4/Lab03_Router_Initial_Config_IPv4.pkt) | Perform basic router setup for IPv4 |
| 4 | [Router Initial Config (IPv6)](IPv6/Lab04_Router_Initial_Config_IPv6.pkt) | Perform basic router setup for IPv6 |
| 5 | [Basic Router Security](Security/Lab05_Basic_Router_Security.pkt) | Apply passwords and secure router access |
| 6 | [WAN Serial Config](WAN/Lab06_WAN_Serial_Config.pkt) | Configure serial WAN links and test |
| 7 | [WAN Ethernet Config](WAN/Lab07_WAN_Ethernet_Config.pkt) | Configure Ethernet WAN links and test |
| 8 | [Static Routing (IPv4)](IPv4/Lab08_Static_Routing_IPv4.pkt) | Implement static routes in IPv4 networks |
| 9 | [Static Routing (IPv6)](IPv6/Lab09_Static_Routing_IPv6.pkt) | Implement static routes in IPv6 networks |
| 10 | [RIP Routing (IPv4)](Routing/Lab10_RIP_IPv4.pkt) | Configure RIP protocol on IPv4 routers |
| 11 | [RIPng Routing (IPv6)](Routing/Lab11_RIPng_IPv6.pkt) | Configure RIPng protocol on IPv6 routers |
| 12 | [OSPF Routing (IPv4)](Routing/Lab12_OSPF_IPv4.pkt) | Configure OSPF single‑area IPv4 |
| 13 | [OSPF Multi‑Area (IPv4)](Routing/Lab13_OSPF_MultiArea_IPv4.pkt) | Configure OSPF multi‑area IPv4 |
| 14 | [OSPFv3 Routing (IPv6)](Routing/Lab14_OSPFv3_IPv6.pkt) | Configure OSPFv3 protocol on IPv6 routers |
| 15 | [EIGRP Routing (IPv4)](Routing/Lab15_EIGRP_IPv4.pkt) | Configure EIGRP protocol on IPv4 routers |
| 16 | [EIGRPv6 Routing (IPv6)](Routing/Lab16_EIGRPv6_IPv6.pkt) | Configure EIGRPv6 protocol on IPv6 routers |
| 17 | [Switch Initial Config](Switching/Lab17_Switch_Initial_Config.pkt) | Perform basic switch setup |
| 18 | [VLANs](Switching/Lab18_VLANs.pkt) | Create VLANs and assign switch ports |
| 19 | [Dynamic Trunking Protocol](Switching/Lab19_DTP.pkt) | Configure DTP for trunk negotiation |
| 20 | [VLAN Trunking Protocol (VTP)](Switching/Lab20_VTP.pkt) | Configure VTP domains and modes |
| 21 | [Router on a Stick](Switching/Lab21_Router_on_a_Stick.pkt) | Configure inter‑VLAN routing |
| 22 | [Spanning Tree Protocol](Switching/Lab22_STP.pkt) | Configure and verify STP operation |
| 23 | [PortFast & BPDU Guard](Switching/Lab23_PortFast_BPDU_Guard.pkt) | Enable PortFast and secure with BPDU Guard |
| 24 | [EtherChannel](Switching/Lab24_EtherChannel.pkt) | Bundle links using EtherChannel |
| 25 | [Port Security](Security/Lab25_Port_Security.pkt) | Restrict switch port access with security |
| 26 | [Standard ACL (IPv4)](Security/Lab26_Standard_ACL_IPv4.pkt) | Apply basic IPv4 access control lists |
| 27 | [Standard ACL (IPv4)](Security/Lab27_Standard_ACL_IPv4.pkt) | Additional practice with standard ACLs |
| 28 | [Extended ACL (IPv4)](Security/Lab28_Extended_ACL_IPv4.pkt) | Configure extended IPv4 ACLs |
| 29 | [Extended ACL (IPv4)](Security/Lab29_Extended_ACL_IPv4.pkt) | Additional practice with extended ACLs |
| 30 | [ACL on IPv6](IPv6/Lab30_ACL_IPv6.pkt) | Configure IPv6 access control lists |
| 31 | [Default Routing](Routing/Lab31_Default_Routing.pkt) | Configure default routes on routers |
| 32 | [Static NAT](NAT/Lab32_Static_NAT.pkt) | Map private to public IPs with static NAT |
| 33 | [Port Address Translation (PAT)](NAT/Lab33_PAT.pkt) | Configure PAT for multiple hosts |
| 34 | [GRE Tunneling](Routing/Lab34_GRE_Tunneling.pkt) | Configure Generic Routing Encapsulation |
| 36 | [Cisco Discovery Protocol (CDP)](Services/Lab36_CDP.pkt) | Use CDP to discover neighbors |
| 37 | [Advanced Router Security](Security/Lab37_Advanced_Router_Security.pkt) | Enhance router security with best practices |
| 38 | [DHCP Server & Client](Services/Lab38_DHCP_Server_Client.pkt) | Configure DHCP services and test leases |
| 39 | [Syslog](Services/Lab39_Syslog.pkt) | Configure logging to a Syslog server |
| 40 | [NTP](Services/Lab40_NTP.pkt) | Synchronize devices with Network Time Protocol |
| 42 | [Password Recovery](Security/Lab42_Password_Recovery.pkt) | Recover lost router/switch passwords |
| 43 | [IOS & Config Backup](IOS_Backup/Lab43_IOS_Config_Backup.pkt) | Backup IOS image and configuration files |
| 44 | [IOS Licensing](IOS_Backup/Lab44_IOS_Licensing.pkt) | Explore IOS license management |
| 45 | [PPP Authentication](WAN/Lab45_PPP_Authentication.pkt) | Configure PPP with authentication |
| 46 | [BGP Routing](Routing/Lab46_BGP_Routing.pkt) | Configure Border Gateway Protocol |


---

## 🚀 How to Use
1. Install [Cisco Packet Tracer](ca://s?q=Download_Cisco_Packet_Tracer).  
2. Clone this repository:
   ```bash
   git clone https://github.com/princeweb1/Cisco-PacketTracer-Labs.git
