# 🏢 Employee Database App (Java + JDBC + PostgreSQL)

A simple **CLI-based Employee Management System** built with **Java JDBC** and **PostgreSQL (Supabase)**.  
Supports basic CRUD operations: **Add, View, Update, Delete Employees**.

---

## 🚀 Features
- ➕ Add Employee  
- 📋 View All Employees  
- ✏️ Update Employee Salary  
- ❌ Delete Employee  

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository
```bash
git clone https://github.com/Sadaqath18/Employee-Database-App.git
cd employee-database-app
```

### 2️⃣ Set Up Supabase Database
Go to Supabase and create a project.
Go to Database → Tables → New Table or use SQL Editor and run:

<details> <summary>Click to view SQL code for creating the table</summary>
sql
CREATE TABLE employees (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    department VARCHAR(50),
    salary NUMERIC(12, 2)
);
</details>
You can run this in Supabase SQL Editor or create the table using the Table Editor.

### 3️⃣ Configure Environment Variables
<details> <summary>Click to view .env file details</summary>
Create a .env file in your project root with:

DB_URL=jdbc:postgresql://<your-db-url>:5432/postgres
DB_USER=postgres
DB_PASSWORD=<your-db-password>
Or set environment variables in Eclipse → Run Configurations → Environment tab.

</details>

### 4️⃣ Compile & Run
```bash
javac -d bin src/com/sadaqath/employee/EmployeeDatabaseApp.java
java -cp bin com.sadaqath.employee.EmployeeDatabaseApp
```

---

### 🖥️ Example Usage:

Run the app
Choose options from the menu:

=== Employee Database App ===
1. Add Employee
2. View Employees
3. Update Employee Salary
4. Delete Employee
5. Exit

Follow the prompts to add, view, update, or delete employees.

### Example Interaction 💻
=== Employee Database App ===
- Choose option: 1
- Enter name: John Doe
- Enter department: IT
- Enter salary: 50000
✅ Employee added successfully!

Choose option: 2

📋 Employee Records:
1 | John Doe | IT | 50000.00

---

## 👨‍💻 Author
### S Sadaqath Ulla Qureshi

---

## 🌐 GitHub Profile
### Sadaqath18
