# Employee Management System 🏢

A full-stack web application designed to streamline human resource workflows by managing employee records efficiently. Built using a robust **Spring Boot** backend and a dynamic **React** frontend, this system provides complete CRUD (Create, Read, Update, Delete) capabilities with seamless asynchronous API communication.

---

## 🚀 Features

*   **Dashboard Overview:** View a structured list of all registered employees.
*   **Employee Onboarding:** Add new employees with detailed profiles (Name, Email, Department, Role, etc.).
*   **Profile Management:** Dynamically update existing employee details.
*   **Offboarding/Removal:** Securely delete employee records from the centralized database.
*   **Responsive UI:** A modern, clean, and user-friendly interface optimized for various screen sizes.
*   **Asynchronous REST Client:** Powered by Axios for smooth, page-refresh-free data operations.

---

## 🛠️ Tech Stack

### Frontend
*   **React.js** - Component-based UI rendering
*   **Axios** - Promise-based HTTP client for API interaction
*   **CSS3 / Bootstrap** - Styling and responsive layout design

### Backend
*   **Java (JDK 17+)** - Core programming language
*   **Spring Boot** - Framework for building the REST API
*   **Spring Data JPA** - Object-Relational Mapping (ORM) for database abstraction
*   **MySQL** - Relational database management system

---

## 📐 Architecture Overview

The application follows a standard decoupled Client-Server architecture:

```text
[ React Frontend ]  <--- (HTTP / JSON / Axios) --->  [ Spring Boot REST API ]
                                                              |
                                                       (Spring Data JPA)
                                                              |
                                                       [ MySQL Database ]# Employee Management System 🏢
```
## ⚙️ Getting Started
# Prerequisites
### Ensure you have the following installed on your local machine:

* Node.js (v16 or higher)

* Java Development Kit (JDK 17 or higher)

* Maven

* MySQL Server

## Backend Setup (Spring Boot)
# Clone the repository and navigate to the backend directory:

```Bash
cd employee-management-backend
Configure the MySQL database connection in src/main/resources/application.properties:
```
```Properties
spring.datasource.url=jdbc:mysql://localhost:3306/employee_db?useSSL=false&serverTimezone=UTC
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
# Hibernate properties
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
spring.jpa.hibernate.ddl-auto=update
```
# Run the Spring Boot application using Maven:

```Bash
mvn spring-boot:run
The server will start on port 8080 by default (http://localhost:8080).
```
## Frontend Setup (React)
# Navigate to the frontend directory:

```Bash
cd employee-management-frontend
```
# Install the necessary dependencies (including Axios):
```Bash
npm install
```
# Start the React development server:

```Bash
npm start
```
The client application will launch in your browser at http://localhost:3000
