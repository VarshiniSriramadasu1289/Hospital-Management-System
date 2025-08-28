# 🏥 Hospital Management System (Java + MySQL)

This project is a **Hospital Management System** built in **Java**, with **MySQL** as the database.  
It allows managing doctors, patients, and hospital records in a structured way.

HospitalManagementSystem/
├── Doctor.java       # Defines the Doctor class (attributes & methods for doctor details)
├── Patient.java      # Defines the Patient class (attributes & methods for patient details)
├── HMS.java          # Main driver program - runs the Hospital Management System
├── TestDBC.java      # Tests the MySQL database connection
└── README.md         # Project documentation

## 🛠️ Prerequisites

Before running this project, make sure you have installed the following:

1. **Java JDK (>= 8)**
   - [Download JDK](https://www.oracle.com/java/technologies/javase-downloads.html)  
   - Verify installation:
     ```bash
     java -version
     ```

2. **MySQL Database (>= 5.7)**
   - [Download MySQL Community Edition](https://dev.mysql.com/downloads/mysql/)  
   - Start MySQL service and create a database:
     ```sql
     CREATE DATABASE hospital_db;
     ```

3. **MySQL Connector/J (JDBC Driver)**
   - [Download MySQL Connector/J](https://dev.mysql.com/downloads/connector/j/)  
   - Add the `.jar` file to your project’s classpath.  
     Example (if using command line):
     ```bash
     javac -cp ".;mysql-connector-j-8.0.33.jar" *.java
     java  -cp ".;mysql-connector-j-8.0.33.jar" HMS
     ```

---


📑 File Details

Doctor.java
Contains the Doctor class with attributes like doctor ID, name, specialization, and related methods.
Helps manage doctor-related data inside the hospital system.

Patient.java
Contains the Patient class with attributes like patient ID, name, age, disease, and related methods.
Helps manage patient-related data in the system.

HMS.java
The main application file that provides the menu-driven interface.
It interacts with Doctor and Patient classes and calls database functions if needed.
This is the file you run to start the program.

TestDBC.java
A utility file to test database connectivity.
It uses JDBC to connect to MySQL (hospital_db) and prints whether the connection is successful.

README.md
Documentation file (this file), explaining how to install, set up, and run the project.
