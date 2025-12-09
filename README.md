# HR-Management-System
Here is the **exact README.md** — clean, polished, and ready to paste directly into GitHub.

---

# 🚀 HR Management System (HRMS) – Full Stack Project

A complete **Human Resource Management System** built using **React**, **Spring Boot**, and **MySQL**.
The system supports **multi-company (multi-tenant)** architecture with automated attendance, payroll generation, leave management, and secure role-based access control.

---

## 🌟 Key Highlights

* Multi-tenant platform with company-level data isolation
* Automated attendance + payroll processing using schedulers
* Role-based dashboards (Super Admin, Company Admin, HR, Manager, Employee)
* JWT authentication and secure REST APIs
* Real-time attendance tracking (Clock-In / Clock-Out)
* Downloadable PDF payslips
* Full employee lifecycle management

---

## 🏗️ Tech Stack

### **Frontend**

* React.js
* React Router
* Axios
* Bootstrap 5
* React-Bootstrap
* React-Toastify

### **Backend**

* Spring Boot
* Spring Security + JWT
* Spring Data JPA
* MySQL
* Cron Schedulers
* iText PDF Generator

---

## 🔐 User Roles & Permissions

| Role                | Responsibilities                                          |
| ------------------- | --------------------------------------------------------- |
| **Super Admin**     | Approves/rejects companies, monitors platform             |
| **Company Admin**   | Manages departments, designations, HR, managers           |
| **HR Manager**      | Employee onboarding, attendance & leave approval, payroll |
| **Project Manager** | Manages team attendance & leaves                          |
| **Employee**        | Clock-in/out, apply leave, view/download payslips         |

---

# 🔄 Core Features

## 1️⃣ Authentication & Security

* JWT-based login
* Password hashing (BCrypt)
* Role-based access
* Protected frontend routes

---

## 2️⃣ Attendance Management

* Clock In / Clock Out with timestamps
* Real-time timer updates in UI
* Monthly auto-generation of attendance sheets
* Auto-mark absent employees daily

---

## 3️⃣ Payroll Management

* Auto payroll generation on 1st of every month
* Salary structure calculation (Basic, HRA, Allowances)
* Deductions (PF, TDS, Professional Tax)
* Generate and download PDF payslips

---

## 4️⃣ Leave Management

* Employees submit leave requests
* Managers approve/reject with comments
* Status tracking + notifications

---
.
## 5️⃣ Company Structure

* Manage departments
* Manage designations
* Add and display company holidays

---

# 🧩 System Architecture (Workflow)

```
React UI → Axios → Spring Boot Controller → Service Layer
→ JPA Repository → MySQL Database → JSON Response → UI Update
```

---

# 📁 Database Overview

* Fully normalized schema
* Every table includes `company_id` for tenant separation
* Foreign key constraints
* Soft delete support
* Indexed fields for performance

---

# 🖥️ Frontend Overview

### Important Components

* `RoleNav.jsx` → Automatically loads role-specific navigation
* `EmployeeAttendanceDashboard.jsx` → Real-time attendance calculations
* `ViewEmployeePayslip.jsx` → Load & download PDF payslips
* `EmployeeLeaveManagement.jsx` → Apply/manage leave requests
* `Admin/HR/Manager Modules` → CRUD for employees, departments, holidays

---

# 🚀 Backend Overview

### Controllers

Handle REST endpoints for authentication, employees, attendance, payroll, etc.

### Services

Contain business logic such as attendance validation and payroll calculation.

### Schedulers

* `AttendanceScheduler` – Monthly attendance generation
* `AttendanceAbsentScheduler` – Mark absent employees daily
* `PayslipScheduler` – Auto-generate monthly payslips

---

# 🎯 What Makes This HRMS Special?

* Full automation of attendance & payroll
* Secure, scalable, and multi-tenant architecture
* Professional UI with real-time updates
* Complete employee lifecycle in one system
* Built with enterprise-level engineering practices

---

# 📌 Conclusion

This HRMS is a complete full-stack system.


