# 🔄 EIGRP Routing Lab (CCNA)

## 🎯 Objective

Configure **EIGRP (Enhanced Interior Gateway Routing Protocol)** between routers and verify dynamic routing and neighbor relationships.

---

## 🖼️ Lab Topology

![EIGRP Topology](EIGRP.png)

---

## 🌐 Network Design

| Router | LAN Network      | AS Number|
|--------|------------------|----------|
| CHE    | 192.168.201.0/24 | 100      |
| HYD    | 192.168.202.0/24 | 100      |
| BAN    | 192.168.203.0/24 | 100      |

---

## ⚙️ Configuration Steps

```bash

### 🔴 **CHE Router (AS 100)**

conf t
router eigrp 100
no auto-summary
network 192.168.201.0 0.0.0.255
network 172.16.0.0 0.0.255.255

🔵 HYD Router (AS 100)

conf t
router eigrp 100
no auto-summary
network 192.168.202.0 0.0.0.255
network 172.16.0.0 0.0.255.255
network 172.17.0.0 0.0.255.255

🔵 BAN Router (AS 100)

conf t
router eigrp 100
no auto-summary
network 192.168.203.0 0.0.0.255
network 172.17.0.0 0.0.255.255
network 172.18.0.0 0.0.0.255.255

✅ Verification
Check EIGRP Neighbors
show ip eigrp neighbors

✅ Expected: Neighbor relationships should be formed

Check Routing Table
show ip route

✅ Expected:

Routes should appear with D (EIGRP) code

Test Connectivity
ping 192.168.202.1
ping 192.168.203.1

✅ Expected:

Successful ping to all networks

⚠️ Troubleshooting
| Issue                 | Solution                       |
| --------------------- | ------------------------------ |
| Neighbors not forming | Check IP connectivity          |
| No routes learned     | Check network command          |
| Wrong routes          | Verify wildcard mask           |
| No ping               | Check interfaces (no shutdown) |

🌍 Real-World Use Case

Cisco enterprise networks
Internal routing in organizations
Fast convergence environments

🎯 Outcome

Understood EIGRP configuration
Verified neighbor relationships
Learned dynamic routing behavior
