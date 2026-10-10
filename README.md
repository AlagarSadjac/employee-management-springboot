# 👥 Employee Management System - REST API

[![Java](https://img.shields.io/badge/Language-Java%2021-orange?logo=java)](https://www.java.com/)
[![Spring Boot](https://img.shields.io/badge/Framework-Spring%20Boot%204.x-6DB33F?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Postman](https://img.shields.io/badge/Testing-Postman-FF6C37?logo=postman&logoColor=white)](https://www.postman.com/)

A high-performance Backend RESTful API built with Java and Spring Boot for managing enterprise employee records. It supports full CRUD operations, connects to PostgreSQL via Spring Data JPA, and features centralized Global Exception Handling for robust API responses.

---

## 📥 API & Project Access
Access the live deployed backend REST API directly on Render or inspect the complete source code on GitHub:

[![Live on Render](https://img.shields.io/badge/Render-Live%20API-46E3B7?style=for-the-badge&logo=render&logoColor=white)](https://employee-crud-rest-api.onrender.com/api/employees)
[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/AlagarSadjac/employee-management-springboot)

---

## 📱 About The Project
Employee Management System API serves as a centralized backend service to streamline employee data operations. Following standard layered MVC architecture, it maps entity models to a relational PostgreSQL database, implements safe data retrieval with custom exception handling, and exposes standard HTTP endpoints for seamless enterprise integration.

---

## ✨ Features
* ➕ **Create Employee:** Add new employee records with attributes like name, email, and department.
* 📋 **Fetch All Records:** Retrieve the complete roster of employees in structured JSON format.
* 🔍 **Retrieve by ID:** Fetch a single employee record by ID with automated validation.
* ✏️ **Update Employee:** Modify and update existing employee attributes in the database.
* 🗑️ **Delete Employee:** Remove employee records safely by their unique primary key ID.
* 🛡️ **Global Exception Handling:** Implements @ControllerAdvice and custom ResourceNotFoundException to return clear HTTP 404 responses for invalid IDs.

---

## 🛠️ Built With
* **Language:** Java 21
* **Framework:** Spring Boot 4.x
* **Database:** PostgreSQL / MySQL
* **ORM / Persistence:** Spring Data JPA & Hibernate
* **Boilerplate Reduction:** Lombok (@Data)
* **Exception Handling:** @ControllerAdvice, @ResponseStatus
* **Build Tool:** Maven
* **API Testing Tool:** Postman

---

## 📸 Screenshots
<p align="center">
  <img src="https://github.com/user-attachments/assets/693b8f7e-7bfc-47b3-89c7-edc62aca169f" width="48%" alt="GET All Employees" />
  &nbsp;
  <img src="https://github.com/user-attachments/assets/b9ffdbe8-43a1-4395-8560-9076345b8474" width="48%" alt="POST Create Employee" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/151a7f19-4321-4517-bf94-61aa9b458fec" width="48%" alt="PUT Update Employee" />
  &nbsp;
  <img src="https://github.com/user-attachments/assets/855a55c9-65c9-4432-8e58-5cf238c9d753" width="48%" alt="DELETE Employee Record" />
</p>

---

## 🚀 How To Run & API Endpoints

### 📡 API Endpoints Reference (/api/employees)

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| GET | /api/employees | Fetch all registered employees |
| GET | /api/employees/{id} | Fetch a specific employee by ID |
| POST | /api/employees | Create and save a new employee |
| PUT | /api/employees/{id} | Update existing employee details |
| DELETE | /api/employees/{id} | Delete employee record by ID |

---

### ⚙️ How To Run Locally

1. Clone the repository:
   ```bash
   git clone [https://github.com/AlagarSadjac/employee-management-springboot.git](https://github.com/AlagarSadjac/employee-management-springboot.git)
   ```

2. Configure database credentials in `src/main/resources/application.properties`:
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/employee_db
   spring.datasource.username=postgres
   spring.datasource.password=your_password
   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
   ```

3. Run the Spring Boot application using Maven:
   ```bash
   mvn spring-boot:run
   ```

4. Access and test the endpoints via Postman at `http://localhost:8080`.
---

## 🎯 Purpose
To demonstrate a clean, maintainable Spring Boot REST API incorporating standard CRUD patterns, database persistence, and centralized exception handling for enterprise employee record systems.

---

## 🔮 Future Updates
* 🔐 Spring Security integration with JWT authentication
* 📑 Pagination and sorting for employee listings
* 📄 Swagger / OpenAPI interactive documentation

---

## 👨‍💻 Developed By
Alagarsamy — Software Developer

---

## ⭐ Support
If you find this project helpful, please give this repository a Star!
