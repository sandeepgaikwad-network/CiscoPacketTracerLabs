# 💻 Assign IP Address to PC (Packet Tracer)

## 🎯 Objective

Manually configure an IP address, subnet mask, and default gateway on a PC in Cisco Packet Tracer.

---

## ⚙️ Configuration Steps

```bash

### Step 1: Select the PC
- Click on the PC in Packet Tracer.

### Step 2: Open Desktop Tab
- Go to **Desktop → IP Configuration**.

### Step 3: Assign IP Address
- Enter IP Address: 192.168.201.10
- Enter Subnet Mask: 255.255.255.0
- Enter Default Gateway: 192.168.201.1

### Step 4: Verify
- Open **Command Prompt** in Desktop tab.
- Run: ping 192.168.201.1

### Step 5: Follow the same step in another PC in different network ie.. 192.168.202.0/24

✅ Verification
ping 192.168.1.1 → Successful reply confirms connectivity to router.
ping <other PC IP> → Confirms LAN communication.
ping <other network PC IP> → Confirms that 2 networks are having communication with the help of router

|    Issue        |              Solution             |
| --------------- | --------------------------------- |
| Ping fails      | Check IP, mask, and gateway       |
| No connectivity | Ensure cables are correct         |
| Wrong subnet    | Verify subnet mask matches router |

🌍 Real-World Use Case
Assigning static IPs in small office/home networks
Preparing PCs for router/switch connectivity tests
Lab practice for CCNA initial setups

🎯 Outcome
PC configured with IP, subnet mask, and gateway
Verified connectivity with router and LAN devices
Learned manual IP assignment in Packet Tracer
