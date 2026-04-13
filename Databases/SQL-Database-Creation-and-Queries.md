✍️ COPY THIS (Clean Markdown + Your Work)

👉 Based on your lab + refined 👇

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

👉 This database stores all related tables and data.

📌 Step 2: Create Tables

Tables were created based on the normalised structure.

CREATE TABLE CusDetails (
    CustomerID INT PRIMARY KEY,
    CusName VARCHAR(255),
    CusEmail VARCHAR(255),
    CusCity VARCHAR(255),
    CusPhone VARCHAR(255),
    LicenseNumber VARCHAR(255)
);

👉 Primary key ensures each record is unique.

📌 Step 3: Insert Data
INSERT INTO CusDetails VALUES
(1, 'John', 'john@email.com', 'Auckland', '021123456', 'LIC123');

👉 This step populates the database with data.

📌 Step 4: Create Relationships (Foreign Keys)
CREATE TABLE OrdDetails (
    OrderID VARCHAR(255),
    CustomerID INT,
    Rego VARCHAR(255),
    CID VARCHAR(255),

    PRIMARY KEY (OrderID),
    FOREIGN KEY (CustomerID) REFERENCES CusDetails(CustomerID)
);

👉 Foreign keys link tables together.

📌 Step 5: Retrieve Data (SELECT)
Query 1:
SELECT Colour, Model, Fuel
FROM CarDetails
WHERE Year = '2018';
Query 2:
SELECT Model, Colour, Transmission
FROM CarDetails
WHERE Fuel = 'Petrol';
Query 3:
SELECT CusName, CusEmail, LicenseNumber
FROM CusDetails
WHERE CusCity = 'Auckland';

👉 SELECT queries retrieve useful information.

📌 Step 6: Delete Data
DELETE FROM CarDetails
WHERE Year = '1994';
DELETE FROM CarDetails
WHERE Model = 'CX7';

👉 DELETE removes unwanted records.

📌 Step 7: Update Data
UPDATE CusDetails
SET CusEmail = 'ShanDeveza@gmail.com'
WHERE CusName = 'Shan';
UPDATE CusDetails
SET CusPhone = '0215792222'
WHERE CusName = 'Ari';

👉 UPDATE modifies existing data.

📌 Key Concepts Demonstrated
Database creation
Table design
Primary and foreign keys
Data insertion
Data retrieval
Data modification
🔗 Integration with Design
Normalisation → Used to design tables
ER Diagram → Defined relationships
SQL → Implemented the database
📌 Real-world Relevance

SQL is widely used in:

Banking systems
E-commerce platforms
Customer management systems

👉 This lab reflects real-world database operations.

🔥 Important Line

SQL enables efficient creation, management, and querying of structured data in databases.

🧠 Simple Understanding

SQL = “create, store, and manage data in tables”

🎤 Interview Line

SQL is used to create and manage databases by defining tables, inserting data, and retrieving information using structured queries.


---

# 🚀 STEP 2

👉 Commit the file

---

# 💬 NEXT

👉 Say:

**“Next: Backup md”**

---

We finish last file → then your **Databases section = COMPLETE** 💪
