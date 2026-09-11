# MySQL Assignment 1 – DDL Commands & Constraints

## 📌 Assignment Overview

This assignment focuses on **MySQL DDL (Data Definition Language) commands and constraints** using an **Employee Database**.

The assignment demonstrates how to create, modify, rename, truncate, drop, and recreate database objects while applying appropriate constraints for data integrity.

## 🗄️ Database Schema

The database contains three tables:

- `Departments`
- `Location`
- `Employees`

The `Employees` table is related to the `Departments` and `Location` tables through foreign keys.

## 🛠️ DDL Commands

The following DDL commands are covered:

- `CREATE`
- `ALTER`
- `RENAME`
- `TRUNCATE`
- `DROP`

### CREATE

- Create the `employee` database
- Create the `Departments` table
- Create the `Location` table
- Create the `Employees` table

### ALTER

- Add an `email` column to `Employees`
- Modify the `designation` column
- Drop the `age` column
- Rename `hire_date` to `date_of_joining`

### RENAME

- Rename `Departments` to `Departments_Info`
- Rename `Location` to `Locations`

### TRUNCATE

- Remove all records from the `Employees` table while retaining its structure

### DROP

- Drop the `Employees` table
- Drop the `employee` database

## 🔐 Constraints

The database is recreated with the following constraints:

- **PRIMARY KEY** – uniquely identifies records
- **FOREIGN KEY** – establishes relationships between tables
- **NOT NULL** – prevents required fields from being empty
- **UNIQUE** – prevents duplicate values
- **AUTO_INCREMENT** – automatically generates sequential IDs
- **ENUM** – restricts gender values to `M` or `F`
- **CHECK** – ensures employee age is 18 or above
- **DEFAULT** – automatically assigns the current date to `hire_date`

## 🔗 Table Relationships

```text
Departments
     │
     │ department_id
     ▼
 Employees
     ▲
     │ location_id
     │
 Location
