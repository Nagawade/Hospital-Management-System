# 🏥 Hospital Management System (Backend)

A Spring Boot–based Hospital Management System designed to manage users, doctors, and role-based access using JWT authentication.

---

## 🚀 Features
- User Registration & Login
- JWT-based Authentication & Authorization
- Role-based Access Control (ADMIN, DOCTOR, PATIENT)
- Doctor onboarding
- Secure REST APIs
- Clean layered architecture (Controller, Service, Repository)

---

## 🛠 Tech Stack
- Java 17
- Spring Boot
- Spring Security
- JWT (JSON Web Token)
- Hibernate / JPA
- MySQL
- Maven
- Lombok
- ModelMapper

---

## 📂 Project Structure
src/main/java
└── com.springboot.project.hospitalmanagement
├── controller
├── service
├── repository
├── entity
├── dto
├── security
├── exception
└── config


---

## 🔐 Authentication Flow
1. User registers or logs in
2. JWT token is generated
3. Token must be passed in headers:
4. Role-based access is validated

---

## 📡 API Endpoints (Sample)

### Auth
- `POST /auth/signup`
- `POST /auth/login`

### Doctor
- `POST /doctor`
- `GET /doctor`

---

## ⚙️ Configuration
Update `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/hospital_db
spring.datasource.username=root
spring.datasource.password=your_password

jwt.secret=your_secret_key
jwt.expiration=86400000
git clone https://github.com/Nagawade/Hospital-Management-System.git
