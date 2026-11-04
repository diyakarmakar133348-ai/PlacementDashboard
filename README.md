# 🎓 Placement Dashboard using ADO.NET

A C# console-based Placement Dashboard developed using **ADO.NET and SQL Server**. This project helps manage and display student placement information, company details, and placement statistics.

## 📌 Project Overview

The Placement Dashboard provides a simple interface to view placement-related information stored in a SQL Server database.

It automatically creates the database and required tables and inserts sample student and placement records when the application runs for the first time.

## ✨ Features

- 📊 **Placement Summary** – Displays total students, placed students, students not placed, and placement percentage.
- 👨‍🎓 **Student Placement Details** – Displays student information and their placement status.
- 🏢 **Company Details** – Displays company names, job roles, and package details.
- 🔗 **ADO.NET Connectivity** – Uses SQL connections and commands to interact with SQL Server.
- 📋 **Data Controls** – Uses `SqlDataAdapter` and `DataTable` to retrieve and display records.
- 🗄️ **Automatic Database Setup** – Creates the database, tables, and sample records automatically.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| C# | Programming language |
| .NET 10 | Application framework |
| ADO.NET | Database connectivity |
| SQL Server LocalDB | Database management |
| Microsoft.Data.SqlClient | SQL Server connection |
| Visual Studio Code | Code editor |

## 🗂️ Database Structure

**Database:** `PlacementDB`

### 1. Students Table

| Column | Description |
|---|---|
| StudentId | Unique student ID |
| EnrollmentNo | Student enrollment number |
| StudentName | Student name |
| Department | Department name |
| PassingYear | Year of passing |
| IsPlaced | Placement status |

### 2. Placements Table

| Column | Description |
|---|---|
| PlacementId | Unique placement ID |
| StudentId | Student reference |
| CompanyName | Company name |
| JobRole | Job position |
| PackageLPA | Package in LPA |

## ⚙️ Installation and Setup

### Prerequisites

- .NET SDK 10.0
- Visual Studio Code
- SQL Server Express LocalDB
- Git

### Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/Placement-Dashboard.git
```

### Step 2: Open the Project

```bash
cd Placement-Dashboard
```

### Step 3: Install the Required Package

```bash
dotnet add package Microsoft.Data.SqlClient
```

### Step 4: Start SQL Server LocalDB

```bash
sqllocaldb start MSSQLLocalDB
```

### Step 5: Run the Application

```bash
dotnet run
```

The application will automatically create the `PlacementDB` database and its tables if they do not already exist.

## 📊 Sample Placement Statistics

The application initially inserts 8 sample students, including 5 placed students.

| Placement Information | Sample Result |
|---|---:|
| Total Students | 8 |
| Placed Students | 5 |
| Not Placed Students | 3 |
| Placement Percentage | 62.50% |
| Highest Package | 6.00 LPA |

## 🖥️ Application Menu

1. Placement Summary
2. View Student Placement Details
3. View Company Details
4. Exit

## 🎯 Learning Outcomes

- Understanding ADO.NET database connectivity.
- Performing SQL queries using C#.
- Using `SqlConnection`, `SqlCommand`, and `SqlDataAdapter`.
- Retrieving records using `DataTable`.
- Understanding SQL JOIN operations.
- Displaying placement statistics using aggregate functions.

## 📝 Note

This repository contains a **single-file C# console-based implementation** of the Placement Dashboard practical for running in Visual Studio Code.

The original practical aim mentions ASP.NET Web Forms data controls and Crystal Reports. This console adaptation demonstrates the database connectivity and placement data functionality; it does not implement Web Forms GridViews or an actual Crystal Reports `.rpt` file.

## 👩‍💻 Author

**Diya Karmakar**

B.Tech – Computer Science and Engineering

Marwadi University

## 📄 License

This project is created for academic and educational purposes.

© 2026 Diya Karmakar. All Rights Reserved.
