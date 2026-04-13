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

---

## 📌 Restore Process

To simulate data loss, the database can be restored from the backup file.

### Restore Query

```sql
RESTORE DATABASE VMS
FROM DISK = 'C:\Backup\VMS.bak';
```
This restores the database to its previous state.

---

## 📌 Validation

- Backup file successfully created  
- Database restored without errors  
- Data verified after restore  

👉 This confirms successful backup and recovery.

---

## 🔗 Integration with Other Topics

- Cybersecurity → Protects against ransomware and data loss  
- IT Operations → Supports business continuity  
- SQL → Enables backup and restore commands  

---

## 📌 Real-world Relevance

Database backup and recovery are essential in all organisations to ensure data availability and continuity.






