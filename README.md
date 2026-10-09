# 🛒 E-Cart Mobile Store API

[![Java](https://img.shields.io/badge/Language-Java%2017+-orange?logo=java)](https://www.java.com/)
[![Spring Boot](https://img.shields.io/badge/Framework-Spring%20Boot%203.x-6DB33F?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![MySQL](https://img.shields.io/badge/Database-MySQL-4479A1?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![Postman](https://img.shields.io/badge/Testing-Postman-FF6C37?logo=postman&logoColor=white)](https://www.postman.com/)

A robust, enterprise-grade E-commerce Backend REST API developed using Java and Spring Boot. It manages users, dynamic mobile inventories, and order processing with automated transactional business logic.

---

## 📥 API & Collection Access
Test and explore the API endpoints directly using Postman:

[![Run in Postman](https://img.shields.io/badge/Postman-API%20Testing-orange?style=for-the-badge&logo=postman)](https://github.com/AlagarSadjac)

> 💡 **Repository Link:** [Explore Source Code & Documentation](https://github.com/AlagarSadjac)

---

## 📱 About The Project
E-Cart Mobile Store API provides core backend services for an online mobile retail system. It automates inventory tracking, validates inputs, and ensures transaction consistency when processing multi-item customer orders without manual intervention.

---

## ✨ Features
* 👤 **User Management:** Secure user registration and profile management.
* 📦 **Product Catalog:** Comprehensive mobile inventory handling (Name, Specs, Price, and Available Units).
* 🛍️ **Order Placement:** Transactional checkout supporting multiple product quantities.
* 📉 **Smart Stock Management:** Real-time atomic reduction of inventory stock upon order confirmation.
* 💰 **Automated Calculations:** Dynamic price estimation and aggregate billing logic.

---

## 🛠️ Built With
* **Language:** Java 17+
* **Framework:** Spring Boot 3.x
* **Data Access:** Spring Data JPA (Hibernate)
* **Database:** MySQL
* **Build Tool:** Maven
* **API Testing & Verification:** Postman

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

## 🚀 How To Run & Test

### API Endpoints
| HTTP Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/users/register` | Register a new user |
| `POST` | `/api/products` | Add a new product to inventory |
| `POST` | `/api/orders/place` | Place an order & reduce stock |

### Setup Steps
1. Clone the repository and configure your MySQL credentials in `application.properties`.
2. Build and run using `./mvnw spring-boot:run`.
3. Test endpoints using Postman by sending JSON payloads to `http://localhost:8080`.

---

## 🎯 Purpose
Designed to demonstrate backend architectural proficiency, database relation mappings, and transactional data consistency required for high-volume retail environments.

---

## 🔮 Future Updates
* 🔐 Spring Security with JWT Authentication
* 💳 Payment Gateway (Razorpay/Stripe) integration
* 🐳 Docker containerization and Render cloud deployment
* 📄 Swagger / OpenAPI automated interactive docs

---

## ⭐ Support
If you find this backend implementation helpful, please give this repository a **Star (⭐)**!
