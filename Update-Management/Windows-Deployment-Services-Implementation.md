# 🖥️ Windows Deployment Services (WDS) Implementation

## 📌 Overview

Windows Deployment Services (WDS) is used to deploy Windows operating systems over a network.  
In this setup, WDS was installed and configured on a Windows Server to support network-based operating system deployment.

---

## 📌 Purpose

- Deploy Windows without USB or DVD media  
- Centralise operating system images  
- Automate installation  
- Support deployment to multiple machines  

---

## 📌 Prerequisites

Before implementing WDS, the following lab environment was already configured:

### 🔹 Active Directory Domain Services (AD DS)

- Domain Name: `skReMinIT.local`
- Domain Controller: `ReMin-AUK-DC-WS2019U-01`

AD DS provides:
- Authentication
- Authorisation
- Centralised management

---

### 🔹 DNS Configuration

- DNS Server: `192.168.10.1`
- Domain zone configured for `skReMinIT.local`

DNS is required for:
- Name resolution
- Domain communication
- WDS integration

---

### 🔹 DHCP Configuration

- DHCP Server: `192.168.10.1`
- Scope Range: `192.168.10.100 – 192.168.10.200`
- Subnet Mask: `255.255.255.0`
- Gateway: `192.168.10.1`

DHCP is required for:
- Automatic IP address allocation
- PXE boot support

---

### 🔹 Server Configuration

- Static IP assigned: `192.168.10.1`
- Connected to Hyper-V virtual network

---

### 🔹 Network Environment

- Hyper-V virtual switch configured
- Server and client machines connected
- Connectivity verified using ping

---

## ✅ Why These Are Important

WDS depends on:

- **AD DS** → for domain integration  
- **DNS** → for name resolution  
- **DHCP** → for PXE boot and IP assignment  

Without these services, WDS cannot function correctly.

---

## 💾 Additional Storage Configuration

An additional storage volume was configured for WDS image storage.

### Requirements:
- Extra disk or partition
- Formatted with **NTFS**
- Used to store boot and install images

This storage is important because WDS needs a dedicated location to save deployment files and images.

---

## ⚙️ WDS Role Installation

### Steps

1. Open **Server Manager**
2. Click **Add Roles and Features**
3. Select:
   - **Windows Deployment Services**
4. Continue and install the role

### Validation

- WDS role installed successfully
- No installation errors displayed

---

## 🏗️ WDS Role Configuration

### Steps

1. Open **Windows Deployment Services**
2. Right-click the server and select **Configure Server**
3. Choose:
   - **Integrated with Active Directory**
4. Select image storage location
5. Configure PXE response settings
6. Complete the configuration wizard

### Screenshot Placeholders

- WDS configuration wizard
- RemoteInstall path selection
- PXE settings

### Validation

- WDS configured successfully
- Services started correctly
- No warning icons shown in the WDS console

---

## 📡 WDS Validation

The WDS setup was validated by checking:

- WDS service status
- Server configuration in WDS console
- Active Directory integration
- Readiness for PXE-based deployment

### Validation Results

- WDS role operational
- Image storage path available
- Server ready for deployment tasks

---

## 🔧 Optional: Image Capture and Deployment

### What is Sysprep?

**Sysprep (System Preparation Tool)** is a Microsoft utility used to prepare a Windows installation so it can be cloned or deployed to multiple machines.

---

### Why Sysprep is Needed

A Windows installation contains unique information such as:

- Security Identifier (SID)
- Computer name
- User-specific settings

These must be removed before capturing and deploying the image to other systems.

---

### What Sysprep Does

- Removes unique system information
- Resets the Windows installation to a clean state
- Clears hardware-specific and user-specific details
- Prepares the system for imaging and deployment

---

### How It Is Used with WDS

1. Create a reference virtual machine
2. Install Windows and required applications
3. Run **Sysprep**
4. Capture the image
5. Deploy it using WDS

---

## 📌 Outcome

- WDS role installed successfully
- WDS configured and integrated with Active Directory
- Image storage prepared
- Server ready for network-based deployment
- Optional image deployment process understood using Sysprep

---

## 📌 Real-world Relevance

WDS is used in:

- Enterprise IT environments
- Schools and labs
- Large-scale operating system deployments

It helps administrators deploy Windows efficiently across multiple devices.

---

## 🔥 Key Point

Windows Deployment Services enables centralised and automated Windows deployment over a network.

---

## 🧠 Simple Understanding

**WDS = install Windows over the network**

---

## 🎤 Interview Line

I have implemented Windows Deployment Services in a domain environment, including dependency setup, storage preparation, role configuration, and deployment readiness validation.
