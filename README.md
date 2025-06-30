# 📊 SQL Join Practice Project

## 🎯 Objective
Learn to combine data from multiple tables using all SQL JOIN types.

---

## 🛠 Tools
- DB Browser for SQLite
- MySQL Workbench

---

## 📦 Deliverables
- SQL queries demonstrating:
  - `INNER JOIN`
  - `LEFT JOIN`
  - `RIGHT JOIN`
  - `FULL OUTER JOIN` (via simulation)

---

## 🧱 Step 1: Create Tables

```sql
-- Customers table
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    CustomerName VARCHAR(50),
    City VARCHAR(50)
);

-- Orders table
CREATE TABLE Orders (
    OrderID INT PRIMARY KEY,
    OrderDate DATE,
    CustomerID INT,
    Amount DECIMAL(10, 2),
    FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID)
);
