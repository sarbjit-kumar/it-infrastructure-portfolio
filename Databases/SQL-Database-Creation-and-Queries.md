# 🗄️ Based on my Lab
# 🗄️ SQL Database Creation & Query Operations

## 📌 Overview

In this lab, a database named **VMS (Vehicle Management System)** was created using Microsoft SQL Server and SQL Server Management Studio (SSMS).

The process included:
- Creating a database  
- Designing tables based on normalisation  
- Defining primary and foreign keys  
- Inserting data  
- Running SQL queries (SELECT, UPDATE, DELETE)  

---

## 📌 Step 1: Create Database

```sql
CREATE DATABASE VMS;
```
This database stores all related tables and data.

---

## 📌 Step 2: Create Tables

Tables were created based on the normalised structure.

```sql
CREATE TABLE CusDetails (
    CustomerID INT PRIMARY KEY,
    CusName VARCHAR(255),
    CusEmail VARCHAR(255),
    CusCity VARCHAR(255),
    CusPhone VARCHAR(255),
    LicenseNumber VARCHAR(255)
);
```
👉 Primary key ensures each record is unique.

---

## 📌 Step 3: Insert Data

```sql
INSERT INTO CusDetails VALUES
(1, 'John', 'john@email.com', 'Auckland', '021123456', 'LIC123');
```
This step populates the database with data.

---

---

## Step 4: Create Relationships (Foreign Keys)

```sql
CREATE TABLE OrdDetails (
    OrderID VARCHAR(255),
    CustomerID INT,
    Rego VARCHAR(255),
    CID VARCHAR(255),

    PRIMARY KEY (OrderID),
    FOREIGN KEY (CustomerID) REFERENCES CusDetails(CustomerID)
);
```
Foreign keys link tables together.

---


---

## Step 5: Retrieve Data (SELECT)

Query 1:

```sql
SELECT Colour, Model, Fuel
FROM CarDetails
WHERE Year = '2018';
```

Query 2:

```sql
SELECT Model, Colour, Transmission
FROM CarDetails
WHERE Fuel = 'Petrol';
```

Query 3:
```sql
SELECT CusName, CusEmail, LicenseNumber
FROM CusDetails
WHERE CusCity = 'Auckland';
```
---

## Step 6: Delete Data

```sql
DELETE FROM CarDetails
WHERE Year = '1994';
```

```sql
DELETE FROM CarDetails
WHERE Model = 'CX7';
```

DELETE removes unwanted records.

---

## Step 7: Update Data

```sql
UPDATE CusDetails
SET CusEmail = 'ShanDeveza@gmail.com'
WHERE CusName = 'Shan';
```

```sql
UPDATE CusDetails
SET CusPhone = '0215792222'
WHERE CusName = 'Ari';
```
UPDATE modifies existing data.

---
