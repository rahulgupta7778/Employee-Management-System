# 👨‍💼 Employee Management System

A comprehensive console-based Employee Management System developed in **Java** that simulates core Human Resource Management (HRMS) operations using **file handling, employee authentication, attendance management, salary processing, role-based access control, secure password hashing, and persistent data storage**.

The system provides separate **Employee** and **Administrator** modules, enabling secure employee management while maintaining attendance records, salary information, and employee profiles.

---

# ✨ Features

## 👤 Employee Module

* Secure employee login using Employee ID and Password
* SHA-256 encrypted password authentication
* Attendance marking with duplicate attendance prevention
* Password reset functionality
* Employee profile viewing
* Attendance history tracking
* Salary slip generation and viewing
* Secure logout system

---

## 👨‍💼 Administrator Module

* Administrative login access
* Add new employee records
* Delete employee records
* Update employee roles
* Search employee information
* List all employees
* Monitor employee attendance records
* Generate and update employee salaries
* Manage employee database

---

# 💾 File Handling

The project uses text files as a lightweight database for persistent storage.

### Files Used

| File Name        | Purpose                                              |
| ---------------- | ---------------------------------------------------- |
| `empRecord.txt`  | Stores employee details, hashed passwords, and roles |
| `attendance.txt` | Stores employee attendance records with timestamps   |
| `salary.txt`     | Stores employee salary information and salary slips  |

---

# 🔐 Security Features

The system incorporates security mechanisms to protect employee data and authentication processes.

### Password Security

* SHA-256 password hashing
* Passwords are never stored in plain text
* Secure password verification during login
* Secure password reset functionality

### Access Control

* Separate Employee and Administrator modules
* Restricted administrative operations
* Authentication-based access control
* Employee-specific profile and salary access

---

# 📅 Attendance Management

### Attendance Features

* Daily attendance marking
* Duplicate attendance prevention
* Attendance timestamp recording
* Employee attendance history tracking
* Attendance count calculation

Each attendance entry is automatically stored with:

* Employee ID
* Date
* Time

Example:

```text
101|20-06-2026 09:15:23
```

---

# 💰 Salary Management

### Salary Components

* Base Salary
* House Rent Allowance (HRA)
* Medical Allowance
* Loss of Pay Calculation
* Net Salary Calculation

### Salary Formula

```text
Net Salary =
(Base Salary + HRA + Medical Allowance)
- Loss of Pay
```

The system automatically generates salary slips containing:

* Employee ID
* Present Days
* Base Salary
* HRA
* Medical Allowance
* Loss in Pay
* Net Payment

---

# 📋 Employee Operations

### Employee Functions

* Login Authentication
* Attendance Marking
* Password Change
* Profile Viewing
* Salary Slip Viewing

### Administrator Functions

* Add Employee
* Delete Employee
* Update Employee Role
* Search Employee
* List Employees
* Attendance Monitoring
* Salary Updates

---

# ⚠️ Validation & Error Handling

The project includes extensive validation and exception handling to ensure data consistency and application reliability.

### Input Validation

* Duplicate Employee ID prevention
* Employee existence verification
* Attendance duplication prevention
* Salary day validation (0–30 days)
* Invalid menu choice handling
* Login credential validation

### Exception Handling

* File not found handling
* File read/write error handling
* Invalid record handling
* Authentication failure handling
* Data parsing exception handling

---

# 🧠 Concepts Used

* Object-Oriented Programming (OOP)
* File Handling
* Authentication Systems
* Password Hashing (SHA-256)
* Role-Based Access Control
* Exception Handling
* Collections Framework (`ArrayList`)
* Data Persistence
* Input Validation
* Salary Processing Logic
* Attendance Management Systems
* Date & Time API (`LocalDateTime`, `DateTimeFormatter`)
* Console-Based User Interface Design

---

# 🛠️ Technologies Used

* Java
* Java Collections Framework
* Java File Handling APIs
* Java Security API (`MessageDigest`)
* Java Time API
* BufferedReader
* BufferedWriter
* Scanner Class

---

# 🚀 How to Run

## Compile the Program

```bash
javac EMPLOYEE_MANAGEMENT_SYSTEM.java
```

## Run the Program

```bash
java EMPLOYEE_MANAGEMENT_SYSTEM
```

---

# 📁 Required Files

The system will automatically create files when records are added. However, the following files are used during execution:

* `empRecord.txt`
* `attendance.txt`
* `salary.txt`

---

# 🔒 Password Hashing Implementation

Passwords are secured using the SHA-256 hashing algorithm.

Example:

```text
Password:
rahul123
```

Stored as:

```text
27cc6994b67f8f8a2f5b4e15fc4f7869d8b4d34c7f8b49e4a94dfd2d4f84b5fd
```

This ensures that actual employee passwords are never stored directly in the system.

---

# 🎯 Learning Outcomes

This project helped in understanding practical implementations of:

* Employee Management Systems
* Human Resource Management Logic
* Secure Authentication Mechanisms
* Password Hashing Techniques
* File-Based Database Simulation
* Attendance Tracking Systems
* Salary Processing Systems
* Data Persistence Techniques
* Role-Based Access Control
* Exception Handling Strategies
* Real-World Console Application Development

---

# 📸 Sample Workflow

### Employee Side

```text
Login
   ↓
Mark Attendance
   ↓
View Profile
   ↓
View Salary Slip
   ↓
Logout
```

### Administrator Side

```text
Admin Login
   ↓
Add / Update / Delete Employees
   ↓
Track Attendance
   ↓
Generate Salary Records
   ↓
Manage Employee Database
```

---

# 👨‍💻 Developed By

## Rahul Gupta
---

# 📖 Project Overview

This project was developed as a practical implementation of a real-world Employee Management System using Java. The primary objective was to simulate HR management operations while gaining hands-on experience in authentication systems, secure password storage, file handling, attendance management, salary processing, and persistent data storage.

The project demonstrates how core Java concepts can be used to build a complete HRMS application without relying on external databases, making it an excellent learning project for understanding software development, security fundamentals, and enterprise application design.
