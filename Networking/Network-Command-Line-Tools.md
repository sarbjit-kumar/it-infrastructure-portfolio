# 🖥️ Network Command-Line Tools

## 📌 Overview

Network command-line tools are used to test, troubleshoot, and analyse network connectivity and configurations.

These tools help administrators quickly identify and resolve network issues.

---

## 📌 Purpose

- Test network connectivity  
- View and manage IP configuration  
- Diagnose network issues  
- Analyse traffic and connections  

---

## 🔧 Common Network Command-Line Tools

---

### 🔹 ping

**Description:**  
Tests connectivity between two devices on a network.

**Protocol Used:**  
ICMP (Internet Control Message Protocol)

**Use Cases:**
- Check if a device is reachable  
- Verify network connectivity  
- Identify packet loss or delay  

**Example:** ping google.com


---

### 🔹 ipconfig

**Description:**  
Displays and manages IP configuration of a system.

**Use Cases:**
- View IP address, subnet mask, and gateway  
- Troubleshoot network issues  
- Renew or release IP address  

**Example:** ipconfig


---

### 🔹 tracert

**Description:**  
Shows the path packets take from source to destination.

**Protocol Used:**  
ICMP

**Use Cases:**
- Identify network delays  
- Locate where connection fails  
- Analyse routing path  

**Example:** tracert google.com


---

### 🔹 netstat

**Description:**  
Displays active network connections and open ports.

**Protocols Used:**  
TCP / UDP

**Use Cases:**
- Monitor active connections  
- Identify open ports  
- Detect suspicious activity  

**Example:** netstat -an


---

### 🔹 nslookup

**Description:**  
Queries DNS to resolve domain names to IP addresses.

**Protocol Used:**  
DNS (Domain Name System)

**Use Cases:**
- Troubleshoot DNS issues  
- Verify domain-to-IP mapping  

**Example:** nslookup google.com


---

### 🔹 flushdns

**Description:**  
Clears the DNS cache stored on the system.

**Use Cases:**
- Resolve website access issues  
- Remove outdated DNS records  
- Fix DNS-related errors  

**Example:** ipconfig /flushdns


---

## 🧠 Key Difference

- **Protocols** = rules of communication (ICMP, DNS, TCP)  
- **Tools** = commands used to test or view those protocols  

---

## 📌 Real-world Relevance

These tools are widely used in:

- IT support  
- Network administration  
- Troubleshooting connectivity issues  

They provide quick and effective diagnosis of network problems.

---

## 🔥 Key Point

Command-line tools are essential for diagnosing and resolving network issues efficiently.

---

## 🎤 Interview Line

I have used command-line tools such as ping, ipconfig, tracert, netstat, and nslookup to troubleshoot network connectivity, IP configuration, and DNS issues.


