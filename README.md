# 🛒 E-Cart Mobile Store API

[![Java](https://img.shields.io/badge/Language-Java%2017+-orange?logo=java)](https://www.java.com/)
[![Spring Boot](https://img.shields.io/badge/Framework-Spring%20Boot%203.x-6DB33F?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![PostgreSQL](https://img.shields.io/badge/Database-PostgreSQL-336791?logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Postman](https://img.shields.io/badge/Testing-Postman-FF6C37?logo=postman&logoColor=white)](https://www.postman.com/)

A high-performance E-Commerce Backend REST API built with Java and Spring Boot to manage online mobile retail operations. It utilizes PostgreSQL for robust relational data storage, offering automated inventory handling, customer authentication, and transactional order fulfillment.

---

## 📥 API & Project Access
Clone the project repository or inspect the complete backend source code directly on GitHub:

[![GitHub Repository](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/AlagarSadjac/e-cart-mobile-store-springboot)

---

## 📱 About The Project
E-Cart Mobile Store API serves as the centralized backend service for an e-commerce platform specializing in mobile devices. It maps clean relational entities using JPA/Hibernate, connects to PostgreSQL for structured data integrity, provides full CRUD endpoints for product stocks, manages customer accounts, and ensures data consistency during checkout.

---

## ✨ Features
* 👤 **User Management & Auth:** Handles user registration (`/register`), login verification (`/login`), and fetches account records.
* 📦 **Product Catalog Management:** Full lifecycle management of mobile models (Create, Read, Update, Delete) with price and stock monitoring.
* 🛍️ **Transactional Order Placement:** Seamless checkout linking registered users to selected products with order timestamps.
* 📉 **Automated Stock Deduction:** Automatically computes and updates available product inventory upon every successful order.
* 💰 **Dynamic Price Calculation:** Evaluates `totalPrice` instantly based on unit price and ordered quantity.

---

## 🛠️ Built With
* **Language:** Java 17+
* **Framework:** Spring Boot 3.x
* **Database:** PostgreSQL
* **ORM / Persistence:** Spring Data JPA (Hibernate) & Jakarta Persistence
* **Boilerplate Reduction:** Lombok (`@Data`, `@Entity`)
* **Build Tool:** Maven
* **API Testing Tool:** Postman

---

## 📸 Screenshots
<p align="center">
  <img src="https://github.com/user-attachments/assets/6b56458f-837d-47b9-9071-ed00c1e844d1" width="48%" alt="Postman Endpoint 1" />
  &nbsp;
  <img src="https://github.com/user-attachments/assets/ac05803d-df56-49b0-b319-3b1574bc6f8f" width="48%" alt="Database Schema" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/1f3ff883-633d-4403-b3c7-42973d7d2489" width="48%" alt="Order Placement Flow" />
  &nbsp;
  <img src="https://github.com/user-attachments/assets/75d5ce11-2080-46cb-8301-12ea3af52a23" width="48%" alt="Product Inventory API" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/ed5afd3a-3cfa-440d-8fbb-286cb3268d63" width="48%" alt="Stock Deduction Verification" />
  &nbsp;
  <img src="https://github.com/user-attachments/assets/c35517b5-5ecf-4d18-a47f-0cc5e2b08189" width="48%" alt="Execution Logs" />
</p>

---

## 🚀 How To Run & API Endpoints

### 📡 API Endpoints Reference

#### 1. User Endpoints (`/api/users`)
* `GET /api/users` - Fetch all registered users
* `POST /api/users/register` - Register a new customer
* `POST /api/users/login?email={email}&password={password}` - Authenticate existing customer

#### 2. Product Endpoints (`/api/products`)
* `GET /api/products` - Retrieve list of available products
* `POST /api/products` - Add a new product to inventory
* `PUT /api/products/{id}` - Update existing product specifications/stock
* `DELETE /api/products/{id}` - Remove a product from catalog

#### 3. Order Endpoints (`/api/orders`)
* `GET /api/orders/all` - List all placed customer orders
* `POST /api/orders/place` - Place a new order & auto-deduct stock

---

### ⚙️ How To Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/AlagarSadjac/e-cart-mobile-store-springboot.git
   ```
2. Configure PostgreSQL settings in `src/main/resources/application.properties`:
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/ecommerce_db
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
To implement and demonstrate a clean, scalable RESTful API architecture following MVC principles, JPA entity associations (`@ManyToOne`), and automated transactional database updates backed by PostgreSQL.

---

## 🔮 Future Updates
* 🔐 Spring Security with JWT (JSON Web Tokens) role-based authorization
* 📄 Swagger / OpenAPI interactive UI documentation
* 🔍 Advanced pagination and filter queries for product inventory

---

## ⭐ Support
If you find this Spring Boot backend implementation helpful, please give this repository a **Star (⭐)**!
