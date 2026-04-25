## 🛠️ Practical Troubleshooting Insights (Lab Update)

This section adds real-world troubleshooting experience from Packet Tracer lab scenarios.

---

### 🔹 ICMP (Ping) — Real Usage

Used to test connectivity between devices.

**Observed Issues:**
- No ping response when IP was incorrect
- No communication when port/interface was OFF

**Learning:**
- Ping is the first and fastest way to check network connectivity

---

### 🔹 DHCP — Real Issues

**Observed Issues:**
- Multiple DHCP servers caused IP conflicts
- DHCP service turned OFF → no IP assignment
- Client using static IP instead of DHCP

**Fix Applied:**
- Disabled extra DHCP servers
- Enabled DHCP on correct server
- Set clients to obtain IP automatically

**Learning:**
- Only ONE DHCP server should be active in a network
- DHCP simplifies IP management

---

### 🔹 DNS — Real Issues

**Observed Issues:**
- Incorrect DNS server IP → communication failure

**Fix Applied:**
- Set correct DNS server IP (e.g. `192.168.10.1`)

**Learning:**
- DNS is required for name resolution
- Wrong DNS can break communication even if IP is correct

---

### 🔹 Default Gateway — Practical Understanding

**Observed Issues:**
- Devices unable to communicate across networks

**Fix Applied:**
- Set correct default gateway

**Learning:**
- Gateway is required to communicate outside local network

---

### 🔹 IP Addressing — Common Mistakes

**Observed Issues:**
- Wrong IP format (e.g. `168.x.x.x`)
- Wrong subnet mask

**Fix Applied:**
- Correct IP range (`192.168.x.x`)
- Correct subnet mask (`255.255.255.0`)

**Learning:**
- IP and subnet must match network design

---

### 🔹 Port / Interface Status

**Observed Issues:**
- FastEthernet / Serial ports were OFF

**Fix Applied:**
- Enabled interfaces

**Learning:**
- Physical/logical interface must be active for communication

---

### 🔹 Wireless Networking

**Observed Issues:**
- Wrong PSK password
- Wireless disabled

**Fix Applied:**
- Correct password
- Enable wireless interface

**Learning:**
- Authentication and configuration must match on both sides

---

### 🔹 Routing Awareness (RIP)

**Observed Issues:**
- Missing network in routing table
- Routers unable to communicate

**Fix Applied:**
- Added correct network in RIP configuration

**Learning:**
- Routing protocols are required for inter-network communication
