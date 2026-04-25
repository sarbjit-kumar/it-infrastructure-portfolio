# 🛠️ Network Troubleshooting Scenarios

## 📌 Overview

Network troubleshooting is the process of identifying, analysing, and resolving issues that prevent devices from communicating properly.

This file summarises real troubleshooting scenarios performed in Cisco Packet Tracer, focusing on IP configuration, DHCP, DNS, routing, and connectivity.

---

## 🎯 Purpose

- Identify common network issues  
- Apply structured troubleshooting methods  
- Resolve connectivity problems  
- Validate communication between devices  

---

## 🔧 Common Network Issues

| Issue Type | Description | Example |
|-----------|------------|--------|
| Incorrect IP Address | Device has wrong IP | `168.168.10.50` → `192.168.10.50` |
| Wrong Subnet Mask | Incorrect network range | Not `255.255.255.0` |
| Wrong Default Gateway | Cannot reach other networks | Missing/wrong gateway |
| DNS Misconfiguration | Domain names not resolving | Wrong DNS IP |
| DHCP Conflict | Multiple DHCP servers | Causes IP conflicts |
| Static vs DHCP Issue | Client not getting IP | Static config instead of DHCP |
| Port Down | Interface disabled | FastEthernet/Serial OFF |
| Wireless Issue | Connection/authentication failure | Wrong PSK |
| Routing Issue | Routers not communicating | Missing RIP configuration |

---

## 🧪 Troubleshooting Method

### 🔹 Standard Approach

1. Check connectivity → `ping`  
2. Check IP configuration → `ipconfig`  
3. Check path → `tracert`  
4. Check DNS → `nslookup`  
5. Check services → DHCP / DNS  
6. Check hardware → Ports, cables, wireless  

---

## 🧩 Scenario 1 — IP Misconfiguration

**Problem:**  
Device cannot communicate.

**Root Cause:**  
Incorrect IP address.

**Solution:**  
- Set correct IP address  
- Verify subnet mask  

**Validation:**  
- Ping successful  
- Correct IP shown in `ipconfig`  

---

## 🧩 Scenario 2 — DHCP Conflict

**Problem:**  
Devices receiving incorrect or no IP.

**Root Cause:**  
Multiple DHCP servers active.

**Solution:**  
- Disable extra DHCP servers  
- Keep only one DHCP server  

**Validation:**  
- Devices receive correct IP  
- DHCP server visible in `ipconfig`  

---

## 🧩 Scenario 3 — Port Down

**Problem:**  
No connectivity.

**Root Cause:**  
Network interface is OFF.

**Solution:**  
- Enable port (FastEthernet / Serial)  

**Validation:**  
- Link becomes active  
- Ping successful  

---

## 🧩 Scenario 4 — Wireless Issue

**Problem:**  
Device cannot connect to wireless network.

**Root Cause:**  
- Wrong PSK password  
- Wireless disabled  

**Solution:**  
- Enter correct password  
- Enable wireless  

**Validation:**  
- Device connects  
- IP assigned via DHCP  

---

## 🧩 Scenario 5 — Routing Issue (RIP)

**Problem:**  
Routers not communicating.

**Root Cause:**  
Missing network configuration in routing table.

**Solution:**  
- Add correct network to RIP  
- Enable required ports  

**Validation:**  
- Router communication successful  
- Ping between networks works  

---

## 🧪 Tools Used

| Tool | Purpose |
|------|--------|
| ping | Test connectivity |
| ipconfig | View IP configuration |
| tracert | Check packet path |
| nslookup | DNS troubleshooting |
| GUI | Device configuration |
| ICMP | Connectivity validation |

---

## ✅ Validation Methods

- Successful ping between devices  
- Correct IP configuration  
- Devices receiving IP from DHCP  
- Network communication restored  

---

## 📌 Outcome

- Network issues identified and resolved  
- Devices communicating successfully  
- Services functioning correctly  
- Troubleshooting process validated  

---

## 🌍 Real-World Relevance

These skills are used in:

- IT support  
- Network administration  
- Enterprise environments  

They help diagnose and resolve real network issues efficiently.

---

## 🔥 Key Point

Network troubleshooting follows a **logical, step-by-step process**.

---

## 🎤 Interview Line

I have performed network troubleshooting in a simulated environment using tools like ping and ipconfig, identified issues such as incorrect IP configuration, DHCP conflicts, and routing problems, and validated solutions through successful connectivity tests.
