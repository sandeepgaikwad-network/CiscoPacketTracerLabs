# 🔗 LAB: EtherChannel

## 🎯 Objective
- Configure Manual EtherChannel between SWITCH‑50 and SWITCH‑51.  
- Verify EtherChannel operation.  
- Configure EtherChannel using PAgP.  
- Configure EtherChannel using LACP.  
- Verify EtherChannel functionality.  

## 🖼️ Lab Topology

![EtherChannel Topology](Etherchannel.png)

## Device Interface Table

| Device     | Interface | IP Address     | Notes                                             |
|------------|-----------|----------------|---------------------------------------------------|
| SWITCH‑50  | VLAN‑1    | 192.168.20.50  | Connected to PCs, EtherChannel ports F0/23 & F0/24 |
| SWITCH‑51  | VLAN‑1    | 192.168.20.51  | Connected to PCs, EtherChannel ports F0/23 & F0/24 |
| PCs        | NIC       | 192.168.20.x   | Assigned IPs in 192.168.20.0/24                   |

## ⚙️ Configuration Steps

## SWITCH 50 Configuration Manual Etherchannel
**Configure Manual EtherChannel**  
SWITCH-50(config)# interface range fa0/23-24  
SWITCH-50(config-if-range)# channel-group 1 mode on

**Verify EtherChannel**  
SWITCH-50# show etherchannel summary

## SWITCH 51 Configuration Manual Etherchannel
**Configure Manual EtherChannel**  
SWITCH-51(config)# interface range fa0/23-24  
SWITCH-51(config-if-range)# channel-group 1 mode on

**Verify EtherChannel**  
SWITCH-51# show etherchannel summary

### Configure EtherChannel with PAgP 
SWITCH-50(config)# interface range fa0/23-24  
SWITCH-50(config-if-range)# channel-group 2 mode desirable

SWITCH-51(config)# interface range fa0/23-24  
SWITCH-51(config-if-range)# channel-group 2 mode auto

### Configure EtherChannel with LACp
SWITCH-50(config)# interface range fa0/23-24  
SWITCH-50(config-if-range)# channel-group 3 mode active

SWITCH-51(config)# interface range fa0/23-24  
SWITCH-51(config-if-range)# channel-group 3 mode passive

**Verify EtherChannel Again**  
SWITCH-50# show etherchannel summary  
SWITCH-51# show etherchannel summary

## Verification Output
- **show etherchannel summary** should display active EtherChannel groups.
- PCs in the same VLAN across switches should communicate successfully.
- Load balancing and redundancy should be confirmed.

## ⚠️ Troubleshooting
| Issue                      | Solution                                                                 |
|----------------------------|--------------------------------------------------------------------------|
| EtherChannel not forming   | Ensure both sides use same mode (on/on, desirable/auto, active/passive)  |
| PCs not communicating      | Verify VLAN configuration and IP assignment                              |
| Interfaces not bundled     | Check speed/duplex consistency across ports                              |

## 🌍 Real-World Use Case
- Link aggregation for increased bandwidth.
- Redundancy in switch interconnections.
- Load balancing across multiple physical links.

## ✅ Outcome
- Configured EtherChannel manually, with PAgP, and with LACP.
- Verified successful bundling of links between SWITCH‑50 and SWITCH‑51.
- Ensured communication and redundancy across the network.

---
## 🙏 Acknowledgment
- This lab guide is part of the CCNA practice series. Thank you for following along and building your skills in networking.

---
## ✍️ Author's Note
- Prepared and documented by **Sandeep Gaikwad** for CCNA lab practice and GitHub repository organization.

---
## ✅ Closing
- Thank you for reviewing this lab manual. Keep practicing consistently — networking mastery comes with hands-on repetition.