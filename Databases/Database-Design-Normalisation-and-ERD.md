# 🧩 Database Design, Normalisation & ER Diagram

## 📌 What is Database Design?

Database design is the process of organising data in a structured way so that it can be stored, accessed, and managed efficiently.

It ensures:
- Data consistency  
- Reduced redundancy  
- Better performance  
- Easy data management  

---

## 📌 What is Normalisation?

Normalisation is the process of organising data into multiple related tables to reduce duplication and improve data integrity.

👉 Goal:
- Remove redundant data  
- Ensure consistency  
- Improve efficiency  

---

## 📌 First Normal Form (1NF)

1NF is the first step of normalisation.

### Rules:
- Each column contains atomic (single) values  
- No repeating groups  
- Each record is unique  

👉 Data is cleaned and structured into basic tables.

---

## 📌 Second Normal Form (2NF)

2NF builds on 1NF.

### Rules:
- Must be in 1NF  
- Remove partial dependency  
- Data must depend on the full primary key  

👉 Data is split into multiple related tables.

---

## 📌 Purpose of Normalisation

- Avoid duplicate data  
- Improve data accuracy  
- Simplify updates  
- Maintain data integrity  

---

## 📌 Entities Identified

From the Vehicle Management System dataset:

- Customer  
- Vehicle  
- Company / Details  
- Orders  

👉 These represent real-world objects in the system.

---

## 📌 Attributes & Keys

### Example: Customer Table

- CustomerID (Primary Key)  
- Name  
- Email  
- City  
- Phone  

👉 Primary key uniquely identifies each record.

---

## 📌 Relationships

Entities are connected using relationships:

- One customer → many orders  
- One vehicle → many orders  

👉 Implemented using foreign keys.

---

## 📌 ER Diagram

An ER (Entity Relationship) diagram visually represents:
- Entities  
- Attributes  
- Relationships  

👉 It helps plan the database before implementation.

---

## 📌 Cardinality & Constraints

Cardinality defines relationships:

- One-to-One (1:1)  
- One-to-Many (1:N)  
- Many-to-Many (M:N)  

Constraints ensure:
- Data accuracy  
- Valid relationships  

---

## 📌 Data Models (Connection)

- Conceptual → What data is needed  
- Logical → Tables and relationships  
- Physical → Actual database implementation  

---

## 🔗 Integration with SQL

This design was used to:
- Create database (VMS)  
- Create tables  
- Define keys  
- Insert and retrieve data  

👉 Normalisation → ER Diagram → SQL Implementation

---

## 🔥 Important Line

Normalisation organises data efficiently by reducing redundancy and improving data integrity.

---

## 🧠 Simple Understanding

Normalisation = “break data into clean, related tables”

---

## 🎤 Interview Line

Normalisation is the process of structuring a database to minimise redundancy and improve data integrity by organising data into related tables.
