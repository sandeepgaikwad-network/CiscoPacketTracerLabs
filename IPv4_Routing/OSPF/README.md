# OSPF (Single Area) Routing Lab (CCNA)

## 🎯 Objective
Configure OSPF (Open Shortest Path First) in a single area (Area 0) and verify neighbor formation and routing table updates.

---

## 🖼️ Lab Topology

![OSPF Topology](OSPF.png)

---

## 🌐 Network Design

| Router | LAN Network        | OSPF Area |
|--------|-------------------|----------|
| CHE    | 192.168.201.0/24  | Area 0   |
| HYD    | 192.168.202.0/24  | Area 0   |
| BAN    | 192.168.203.0/24  | Area 0   |

---

## ⚙️ Configuration Steps
```bash

### 🔴 **CHE Router (Area 0)**

conf t
router ospf 1
network 192.168.201.0 0.0.0.255 area 0
network 172.16.0.0 0.0.0.3 area 0
network 172.18.0.0 0.0.0.3 area 0
