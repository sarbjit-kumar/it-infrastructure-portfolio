# 💾 SQL Database Backup & Restore

## 📌 Overview

In this lab, backup and restore operations were performed on the **VMS (Vehicle Management System)** database to ensure data protection and recovery.

---

## 📌 Importance of Backup

Databases store critical business data. Loss of data can lead to:

- Business disruption  
- Financial loss  
- Loss of customer trust  

👉 Backup ensures data can be recovered in case of failure.

---

## 📌 Common Causes of Data Loss

- Human error (accidental deletion)  
- Hardware failure  
- Power failure  
- Cyber attacks (ransomware, SQL injection)  
- Natural disasters  

---

## 📌 Backup Process

Before performing backup, appropriate folder permissions were configured to allow SQL Server to store backup files.

### Backup Query

```sql
BACKUP DATABASE VMS
TO DISK = 'C:\Backup\VMS.bak';
```
This creates a full backup of the database.
