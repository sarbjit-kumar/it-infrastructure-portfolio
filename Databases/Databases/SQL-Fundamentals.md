# 🗄️ SQL Fundamentals

## 📌 What is SQL?

SQL (Structured Query Language) is a database language used to create, update, delete, and retrieve data from a database.

In simple terms, SQL is used to communicate with databases. Most websites and applications use databases, and SQL is used to access and manage that data.

👉 Client applications send SQL queries to the database server, which processes them and returns results.

---

## 🎯 Purpose of SQL in IT Industry

SQL is important because:

- It allows applications to store and manage data  
- It helps retrieve useful information for decision-making  
- It supports modern systems like websites, apps, and business tools  
- It enables efficient handling of large data  

👉 Without SQL, most IT systems cannot function properly.

---

## 📌 Role of SQL Queries

SQL queries are commands used to interact with databases.

They allow:
- Retrieving data → `SELECT`  
- Inserting data → `INSERT`  
- Updating data → `UPDATE`  
- Deleting data → `DELETE`  

👉 Queries act as a bridge between users/applications and the database.

---

## 📌 Common SQL Commands

- `CREATE DATABASE` → Create database  
- `CREATE TABLE` → Create table  
- `ALTER` → Modify structure  
- `DROP` → Delete table/database  
- `SELECT` → Retrieve data  
- `INSERT` → Add data  
- `UPDATE` → Modify data  
- `DELETE` → Remove data  

---

## 📌 DDL vs DML

### 🔹 DDL (Data Definition Language)
Used to define database structure.

**Examples:**
- `CREATE`
- `ALTER`
- `DROP`
- `TRUNCATE`

👉 DDL affects structure and is auto-committed.

---

### 🔹 DML (Data Manipulation Language)
Used to manage data inside tables.

**Examples:**
- `SELECT`
- `INSERT`
- `UPDATE`
- `DELETE`

👉 DML works on data and can be rolled back.

---

## 🔄 Key Difference

| DDL | DML |
|-----|-----|
| Works on structure | Works on data |
| Auto-committed | Not auto-committed |
| Cannot rollback | Can rollback |
| No WHERE clause | Uses WHERE clause |

---

## 📌 Primary Key vs Foreign Key

### 🔹 Primary Key
- Uniquely identifies each record  
- No duplicate or null values  
- Only one per table  

---

### 🔹 Foreign Key
- Links tables together  
- Refers to primary key in another table  
- Can have duplicate values  

---

## 📌 Query Optimisation (Simple)

Query optimisation is the process of executing SQL queries in the most efficient way.

👉 Goal:
- Reduce CPU usage  
- Reduce memory usage  
- Reduce disk I/O  

### Types:
- Heuristic optimisation → Rule-based  
- Cost-based optimisation → Chooses lowest-cost plan  

---

## 📌 Data vs Information

### Data
- Raw facts (numbers, values)  
- No meaning on its own  

### Information
- Processed data  
- Useful for decision-making  

👉 Data → processed → Information

---

## 📌 Database Management System (DBMS)

A DBMS is software used to manage databases.

It allows:
- Creating databases  
- Storing data  
- Retrieving data  
- Updating data  

### Examples:
- Microsoft SQL Server  
- MySQL  
- Oracle  
- PostgreSQL  

---

## 📌 Data Models (Overview)

A data model defines how data is structured and related.

### Types:
- Conceptual → What data is needed  
- Logical → Structure of data  
- Physical → How data is stored  

---

## 🔥 Important Line

SQL is the foundation of database systems and is essential for managing and retrieving structured data efficiently.

---

## 🧠 Simple Understanding

SQL = “language to talk to database”

---

## 🎤 Interview Line

SQL is a standard language used to interact with relational databases, allowing users to create, retrieve, update, and manage data efficiently.
