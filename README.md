# Vehicle-Rental-System-Java-JDBC
Console-based Vehicle Rental System using Java, JDBC, and MySQL with CRUD operations and relational database design.

# 🚗 Vehicle Rental System (Java + JDBC)

## 📌 Project Overview
The **Vehicle Rental System** is a console-based Java application that manages vehicle rentals efficiently using JDBC and MySQL.
It allows users to perform CRUD operations on vehicles, customers, and rentals while maintaining data integrity using foreign key constraints.

## 🛠️ Technologies Used
* ☕ Java
* 🔗 JDBC (Java Database Connectivity)
* 🗄️ MySQL
* 💻 Console-based UI

## ✨ Features
* 🚘 Manage Vehicles (Add, View, Update, Delete)
* 👤 Manage Customers (Add, View, Update, Delete)
* 📅 Manage Rentals (Book, View, Update, Delete)
* 🔗 Foreign Key Relationships (Customers ↔ Rentals ↔ Vehicles)
* 📊 Data Retrieval using SQL JOIN
* ⚙️ Automatic Table Creation
* 🔒 Data Integrity using Constraints

## 🧩 Database Structure

### 🚘 Vehicles
* vehicle_id (Primary Key)
* model
* type
* availability
* price_per_day

### 👤 Customers
* customer_id (Primary Key)
* name
* license_number (Unique)
* contact

### 📅 Rentals
* rental_id (Primary Key)
* customer_id (Foreign Key)
* vehicle_id (Foreign Key)
* start_date
* end_date
* status

## ▶️ How to Run the Project
1. Install MySQL and create database:
   ```sql
   CREATE DATABASE vehicleproject;
   ```
2. Update DB credentials in code:
   ```java
   String url = "jdbc:mysql://localhost:3306/vehicleproject";
   String user = "root";
   String password = "root";
   ```
3. Compile and run:
   ```bash
   javac VehicleRentalSystem.java
   java VehicleRentalSystem
   ```
   
## ⚠️ Important Notes
* This is a **console-based application**, not a web application
* It runs locally using MySQL database
* Not deployable on platforms like Vercel

## 🚀 Future Enhancements
* ✅ Convert to GUI (Java Swing / JavaFX)
* 🌐 Build Web Version (React + Backend)
* 💰 Add Billing Calculation
* 🔍 Search & Filter Features
* 📈 Reports and Analytics

## 🎯 Learning Outcomes
* JDBC connectivity with MySQL
* SQL CRUD operations
* Database normalization and relationships
* Handling real-world scenarios like rentals and availability

## 👩‍💻 Author
**Kiruthika Citharanjan**

## ⭐ If you like this project
Give it a ⭐ on GitHub! 
