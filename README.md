# 🐾 DogRestAPI-SpringBoot

This is a backend project built using **Spring Boot** that provides a RESTful API for managing dog-related data. It demonstrates clean backend architecture, testing practices, and integration with an in-memory database.

---

## 📌 Features

- 🐶 RESTful API endpoints for dog data (name, breed, etc.)
- 🗃️ In-memory H2 database integration
- 🧪 Unit and Integration testing using Spring Boot Test
- 📄 API documentation via Springdoc OpenAPI/Swagger UI
- 💡 Clean architecture using service and controller layers

---
## 🔧 Technologies Used

- **Java 21**
- **Spring Boot 3**
- **Spring Web**
- **Spring Data JPA**
- **H2 Database**
- **Springdoc OpenAPI**
- **JUnit 5**

---

## 📂 Project Structure

```bash
src/
├── main/
│   ├── java/
│   │   └── com.example.DogRestApi/
│   │       ├── config/               # Spring Security & Swagger config
│   │       │   ├── SpringSecurityConfig.java
│   │       │   └── SwaggerConfig.java
│   │       ├── entity/               # Dog entity
│   │       │   └── Dog.java
│   │       ├── repository/           # JPA repository interface
│   │       │   └── DogRepository.java
│   │       ├── service/              # Service interface + implementation + exception
│   │       │   ├── DogService.java
│   │       │   ├── DogServiceImpl.java
│   │       │   └── DogNotFoundException.java
│   │       ├── web/                  # REST controller
│   │       │   ├── DogController.java
│   │       │   └── DogRestApiApplication.java
│   └── resources/
│       ├── application.properties    # App configuration
│       └── data.sql                  # Initial data load
└── test/
    └── java/
        └── com.example.DogRestApi/
            └── DogRestApiApplicationTests.java
