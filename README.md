
# Spring MVC 5 + Hibernate 5 + JSP + MySQL

This project is a **Spring MVC 5** application using **Hibernate 5** as the ORM and **MySQL** as the database, with **JSP** as the view layer. The application demonstrates a basic CRUD operation for managing entities in a MySQL database, showcasing integration between these technologies in a web application.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Running the Application](#running-the-application)
- [Usage](#usage)

## Features
- CRUD operations for managing entities in the database.
- Integration of Spring MVC and Hibernate.
- MySQL database configuration.
- JSP view for displaying data and interacting with the application.
- Simple form handling and data validation.

## Technologies Used
- **Spring MVC 5**
- **Hibernate 5**
- **JSP** (Java Server Pages)
- **MySQL** for the database
- **Java** (JDK 8 or higher)

## Project Structure
```
src/main/java
    ├── config          # Spring and Hibernate configuration
    ├── controller      # Controller classes for handling requests
    ├── dao             # Data access objects for database interactions
    ├── model           # Entity classes representing database tables
    └── service         # Service layer for business logic
src/main/resources
    └── hibernate.cfg.xml  # Hibernate configuration file
src/main/webapp
    ├── WEB-INF
    │   ├── jsp         # JSP views
    │   └── web.xml     # Application deployment descriptor
```

## Prerequisites
- **JDK 8** or higher
- **Maven** for dependency management
- **MySQL** database

## Setup
1. **Clone the repository**:
   ```bash
   git clone https://github.com/rabiyag/springmvc5-hibernate5-jsp-mysql.git
   cd springmvc5-hibernate5-jsp-mysql
   ```

2. **Configure MySQL Database**:
   - Create a database in MySQL (e.g., `springmvc_hibernate`).
   - Update the MySQL database credentials in `hibernate.cfg.xml` (located in `src/main/resources`).

3. **Build the project with Maven**:
   ```bash
   mvn clean install
   ```

## Running the Application
1. **Start MySQL** and ensure your database is running.
2. **Run the application**:
   ```bash
   mvn spring-boot:run
   ```
3. **Access the application**:
   - Open a browser and go to `http://localhost:8080`.

## Usage
- The home page will display the list of entities.
- Use the form to add new records to the database.
- Edit and delete operations are available to manage existing records.
