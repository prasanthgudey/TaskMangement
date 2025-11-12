# 🧭 TaskFlow Management System

A full-stack demo project built using **ASP.NET Core Web API** and **Blazor WebAssembly**, designed to practice enterprise-grade architecture patterns such as **DDD**, **CQRS**, **Repository Pattern**, and **Clean Architecture**.

This project simulates a real-world **team task management platform** where users can create, assign, and track tasks within different projects.

---

## 🚀 Tech Stack

### **Backend (Server)**
- ASP.NET Core 8 Web API  
- Entity Framework Core (Code-First + Migrations)  
- MediatR (for CQRS pattern)  
- FluentValidation  
- Serilog (for logging)  
- AutoMapper  
- JWT Authentication & Identity

### **Frontend (Client)**
- Blazor WebAssembly  
- Bootstrap / Tailwind CSS  
- JWT Auth integration  
- HttpClient for Web API communication  

---

## 🧩 Features

### **Authentication & Authorization**
- Secure login and registration using **JWT tokens**  
- Roles: **Admin** and **Member**

### **Project Management**
- Admin can create, update, delete, and view projects  
- Assign members to projects

### **Task Management**
- Admin or assigned member can:
  - Create a new task under a project
  - Update task status (`Pending`, `InProgress`, `Completed`)
  - Add comments to a task
  - View all tasks within a project

### **Activity Log**
- Every action (Create/Update/Delete) is logged using **Serilog**

### **Validation & Error Handling**
- All input validated using **FluentValidation**
- Centralized **Exception Middleware** for error responses

---

## 🧠 Architecture Overview

This project follows **Domain-Driven Design (DDD)** with **CQRS (Command Query Responsibility Segregation)** to ensure clean separation of concerns.

