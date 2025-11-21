# MySQL Library Database

A complete **Library Management Database** built in **MySQL 8+**.  
This project demonstrates database modeling, relationships, constraints, indexing,  
and real-world SQL reporting queries.

---

## 📂 Project Structure

- `schema.sql` – creates all tables, constraints, indexes  
- `data.sql` – inserts realistic sample data  
- `queries.sql` – useful SELECT queries for analysis and reporting  

---

## 🧱 Database Model

The system includes:

- **authors**  
- **categories**  
- **books**  
- **book_authors** (many-to-many)  
- **members**  
- **loans**  
- **loan_items**

Relations:
- One category → many books  
- One book → many authors (via pivot table)  
- One member → many loans  
- One loan → many loan items → many books  

---

## 🚀 How to Run

1. Create a new MySQL database:
```sql
CREATE DATABASE librarydb;
USE librarydb;
