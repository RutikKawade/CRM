# 📄 CRM Microservices Project

[![Java](https://img.shields.io/badge/Java-17+-blue?logo=java&logoColor=white)](https://www.java.com/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2.0-green?logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![MySQL](https://img.shields.io/badge/MySQL-8.0-blue?logo=mysql&logoColor=white)](https://www.mysql.com/)
[![GitHub](https://img.shields.io/badge/GitHub-RutikKawade-black?logo=github&logoColor=white)](https://github.com/RutikKawade)

---

## 📚 Overview
This **Customer Relationship Management (CRM)** project is built using **Spring Boot** and a **Microservices Architecture**.  
Each service is independent, providing **scalability, maintainability, and easy deployment**.

**Maintained by:** Rutik Kawade  

The project includes the following microservices:

- 👤 **User Management Service**  
- 📞 **Contact Management Service**  
- 🧲 **Lead Management Service**  
- 💰 **Sales Management Service**  
- 📢 **Marketing Campaign Service**  
- 🛠️ **Support Ticket Service**  

All services communicate using **REST APIs**.

---

## 🚀 Technologies Used
- **Backend:** Java 17+, Spring Boot, Spring Web, Spring Data JPA  
- **Database:** MySQL  
- **Communication:** REST APIs (via RestTemplate)  
- **Tools:** Maven, Git, GitHub, Postman  
- **Architecture:** Microservices  

---

## 🧩 Services and APIs

### 1. 👤 User Management Service
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/users/save` | Create a new user |
| GET    | `/users/all` | Get all users |
| GET    | `/users/{userId}` | Get user by ID (and assigned leads) |
| PUT    | `/users/{userId}` | Update user details |
| DELETE | `/users/{userId}` | Soft delete (deactivate user) |
| GET    | `/users/active` | Get all active users |

---

### 2. 📞 Contact Management Service
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/contacts/save` | Create a new contact |
| GET    | `/contacts/new` | Get all contacts |
| GET    | `/contacts/{contactId}` | Get contact by ID |
| PUT    | `/contacts/{contactId}` | Update contact details |
| DELETE | `/contacts/{contactId}` | Delete a contact |

---

### 3. 🧲 Lead Management Service
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/leads/save` | Create a new lead |
| GET    | `/leads/all` | Get all leads |
| GET    | `/leads/{leadId}` | Get lead by ID |
| GET    | `/leads/user/{userId}` | Get leads assigned to a user |
| PUT    | `/leads/{leadId}` | Update lead details |
| DELETE | `/leads/{leadId}` | Delete a lead |

---

### 4. 💰 Sales Management Service
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/sales/save` | Create a new sale |
| GET    | `/sales/all` | Get all sales |
| GET    | `/sales/{saleId}` | Get sale by ID |
| PUT    | `/sales/{saleId}` | Update sale details |
| DELETE | `/sales/{saleId}` | Delete a sale |

---

### 5. 📢 Marketing Campaign Service
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/campaigns/save` | Create a new marketing campaign |
| GET    | `/campaigns/all` | Get all campaigns |
| GET    | `/campaigns/{campaignId}` | Get campaign by ID |
| PUT    | `/campaigns/{campaignId}` | Update campaign details |
| DELETE | `/campaigns/{campaignId}` | Delete a campaign |

---

### 6. 🛠️ Support Ticket Service
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/tickets/save` | Create a new support ticket |
| GET    | `/tickets/all` | Get all support tickets |
| GET    | `/tickets/{ticketId}` | Get ticket by ID |
| GET    | `/tickets/user/{userId}` | Get tickets submitted by a user |
| PUT    | `/tickets/{ticketId}` | Update ticket details or status |
| DELETE | `/tickets/{ticketId}` | Delete a support ticket |

---

## 🔗 Communication Between Services
- **User Service ↔ Lead Service**: Fetch user’s assigned leads  
- **Lead Service ↔ Contact Service**: Link leads with contacts  
- **Lead Service ↔ Sales Service**: Convert leads to sales  
- **User Service ↔ Support Ticket Service**: Manage tickets submitted by users  

Communication is implemented via **Spring RestTemplate**.

---

## ✅ Project Status
- All services completed and tested successfully  
- Database schema and sample data created  
- Ready for **frontend integration**  

---

## 📂 Folder Structure

