# JavaFX MySQL CRUD Application

A desktop application built with **JavaFX** and connected to a **MySQL** database using **JDBC**. This app performs basic **CRUD operations** (Create, Read, Update, Delete) on a student database and displays data in a user-friendly TableView.

## Features

- Add, update, delete, and view student records
- MySQL database integration using JDBC
- JavaFX UI with TableView and form input
- Simple, clean, and easy-to-understand code structure

## Prerequisites

- Java 8 or higher  
- MySQL Server installed and running  
- JavaFX SDK  
- MySQL Connector/J (JDBC Driver)  
- VS Code or any Java IDE

## Setup Instructions

1. Clone or download the project files.
2. Create a folder named `lib/` in your project (if not already there).
3. Place `mysql-connector-java-x.x.x.jar` in the `lib/` folder.
4. Add the JAR to your project’s build path.
5. Create the database:

```sql
CREATE DATABASE school;
USE school;

CREATE TABLE students (
  id INT PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(100),
  email VARCHAR(100),
  age INT
);
