# 🧠 Entity Framework Core 8.0 Hands-on Labs (Retail Inventory System)

This repository contains step-by-step labs completed as part of the DN 4.0 DotNet FSE training. The application simulates a **Retail Inventory System** using **Entity Framework Core 8.0**.

---

## 📋 Lab Index

| Lab No. | Title                                      | Description |
|--------:|--------------------------------------------|-------------|
| Lab 1   | Understanding ORM                          | Introduction to ORM concepts and EF Core structure |
| Lab 2   | Setting Up the Database Context            | Create and configure `AppDbContext` using EF Core |
| Lab 3   | Creating and Applying Migrations           | Use EF CLI to generate and apply schema to SQL Server |
| Lab 4   | Inserting Initial Data                     | Seed initial data into tables using code |
| Lab 5   | Retrieving Data with LINQ                  | Fetch and filter data using LINQ and EF queries |
| Lab 6   | Updating and Deleting Records              | Modify and delete records using EF Core methods |
| Lab 7   | Writing Queries with LINQ                  | Use advanced LINQ queries to sort, filter, and project |

---

## 📦 Technologies Used

- C#
- .NET 8.0
- Entity Framework Core 8.0
- SQL Server LocalDB
- Visual Studio 2022

---

## 📁 Folder Structure

RetailAppEFCore/
│
├── Models/ # Contains Product, Category, Customer, Order classes
├── Migrations/ # EF Core migration files
├── AppDbContext.cs # Database context
├── Program.cs # Console app entry and lab execution
├── RetailAppEFCore.csproj # Project configuration
└── README.md # This file

yaml
Copy
Edit

---

## 🔧 How to Run

1. Clone the repository or open the project in Visual Studio.
2. Run the following EF CLI commands:

```bash
dotnet ef migrations add InitialCreate
dotnet ef database update
Press Ctrl + F5 to execute the app and see lab outputs in the console.

📸 Screenshots & Code Snippets
All lab details with code and screenshots are available in the lab report document:
➡️ EFCore_Lab_Report.docx

✅ Completion Status
 Lab 1: ORM Basics

 Lab 2: AppDbContext Setup

 Lab 3: Migrations

 Lab 4: Seed Data

 Lab 5: Data Retrieval

 Lab 6: Update/Delete

 Lab 7: Advanced LINQ

🧠 Author
Ananya Upadhyay(6364141)
roll no - 22053488
DotNet FSE Track — DN 4.0 Cohort (COGNIIZANT)
KIIT University
