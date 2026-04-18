# 🌐 Subnetting

## 📌 Overview

Subnetting is the process of dividing a larger IP network into smaller subnetworks. It helps organise networks efficiently, improves performance, and reduces unnecessary IP address wastage.

Subnetting is a very important networking skill because it is used in real-world network design, routing, security, and troubleshooting.

---

## 📌 Purpose of Subnetting

Subnetting is used to:

- Improve network performance  
- Reduce broadcast traffic  
- Organise devices into smaller network segments  
- Increase security by separating departments or functions  
- Use IP addresses more efficiently  

---

## 📌 Basic Concepts

| Term | Meaning |
|------|---------|
| Network Address | Identifies the subnet itself |
| Host Address | Identifies a device within the subnet |
| Broadcast Address | Used to send data to all devices in the subnet |
| Subnet Mask | Separates network portion from host portion |
| CIDR Notation | Slash notation showing network bits, e.g. `/24` |

---

## 📌 Example Network

Given network:

- Network Address: `192.168.1.0/24`
- Requirement: 3 departments
- Each department needs 50 hosts

---

## 📌 Step 1: Find Required Host Bits

To support 50 hosts, we use the formula:

`2^n - 2`

We test values:

- `2^5 - 2 = 30` ❌  
- `2^6 - 2 = 62` ✅  

👉 Therefore, **6 host bits** are needed.

---

## 📌 Step 2: Determine New Subnet Mask

Original network = `/24`  
If 6 bits are for hosts, then remaining bits are for network.

👉 New subnet mask = **/26**

Subnet mask in decimal:

`255.255.255.192`

---

## 📌 Step 3: Calculate Subnets

A `/26` subnet gives:

- Total addresses per subnet = 64
- Usable hosts per subnet = 62

### 📊 Subnet Table

| Subnet | Network Address | Usable Host Range | Broadcast Address |
|--------|-----------------|------------------|-------------------|
| Subnet 1 | 192.168.1.0/26 | 192.168.1.1 - 192.168.1.62 | 192.168.1.63 |
| Subnet 2 | 192.168.1.64/26 | 192.168.1.65 - 192.168.1.126 | 192.168.1.127 |
| Subnet 3 | 192.168.1.128/26 | 192.168.1.129 - 192.168.1.190 | 192.168.1.191 |
| Subnet 4 | 192.168.1.192/26 | 192.168.1.193 - 192.168.1.254 | 192.168.1.255 |

---

## 📌 Step 4: Explanation

Each `/26` subnet provides 62 usable IP addresses, which is enough for each department requiring 50 hosts.

This design allows the original `/24` network to be divided efficiently into four smaller subnets.

---

## 📌 Why Subnetting is Useful

| Benefit | Explanation |
|---------|-------------|
| Better Performance | Smaller broadcast domains reduce congestion |
| Better Organisation | Departments can be separated logically |
| Improved Security | Segmentation makes networks easier to control |
| Efficient Address Usage | IP space is used more effectively |

---

## 📌 Real-world Relevance

Subnetting is used in:

- Office networks  
- Schools and universities  
- Data centres  
- Cloud environments  
- Enterprise network design  

👉 It is essential for network engineers, system administrators, and IT support professionals.

---

## 🔥 Important Line

Subnetting improves network efficiency by dividing a larger network into smaller, manageable subnetworks.

---

## 🧠 Simple Understanding

Subnetting = “divide one network into smaller networks”

---

## 🎤 Interview Line

I understand subnetting and can divide networks into smaller subnets using subnet masks and CIDR notation to improve performance, organisation, and efficient IP address usage.
