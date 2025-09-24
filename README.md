# 🚢 Cargo Reservation System

## 📌 Project Purpose

<!-- Cargo Reservation & Tracking System

Developed a Java/Spring Boot application to manage cargo bookings and track shipments, improving operational accuracy.

Designed and maintained SQL/Oracle databases, enabling efficient data retrieval and reporting.

Integrated REST APIs to automate workflows and enhance cargo handling reliability.

Airline Cargo Analytics Dashboard

Built a dashboard to monitor cargo operations and generate actionable insights for airline management.

Aggregated and analyzed data using SQL and Java, providing stakeholders with real-time visibility.

Streamlined reporting workflows, reducing manual analysis and supporting strategic decisions.-->


The **Cargo Reservation System** is a backend web application designed to manage customers, cargo bookingsand track shipments, improving operational accuracy.  
It provides a scalable foundation for handling CRUD operations via REST APIs, supporting both single and bulk data creation.  
The system is built for extensibility, enabling future integration with dashboards and analytics tools to monitor reservations and customers in real-time.

## 🚀 Roadmap

- **Phase 1: Customer CRUD + bulk insertion (✅ Done)**

- **Phase 2: Flight entity & reservations**

- **Phase 3: Booking system**

- **Phase 4: Authentication & roles**

- **Phase 5: Version control & GitHub setup (✅ This phase)**

- **Phase 6: Frontend dashboard & analytics**


## 🛠️ Technologies Used
- **Eclipse Version: 1,103.2 user setup**
- **Java 17** – Core programming language  
- **Spring Boot 3** – Backend framework (REST APIs, dependency injection, JPA)  
- **Spring Data JPA (Hibernate)** – ORM for database access  
- **PostgreSQL** – Relational database  
- **Maven** – Build and dependency management  
- **Postman** – API testing  
- **Git & GitHub** – Version control and repository hosting  

---

## ⚙️ Setup Instructions

### 1. Clone the repository

bash
git clone https://github.com/Marc1401/cargo-reservation-system.git <br>
cd cargo-reservation-system


## Configuraion

Step 1: Install the required technlogies used

- Verify the configuration PATH environment variable for Maven in the terminal: mvn -v
- In the command prompt, create a database called "cargo_db": CREATE DATABASE cargo_db;

Step 2: Initialize Spring Boot Project

1. Go to [Spring Initializr] (https://start.spring.io/)
2. Configure:
  - Project: **Maven**
  - Language: **Java**
  - Spring Boot: 3.5.6
  - Dependencies: 
     - Spring Web → to build REST APIs
     - Spring Data JPA → to interact with the database
     - PostgreSQL Dirver → to connect to PostgreSQL
     - Validation → input validation
     - Lombok → to reduce boilerplate code
     - Spring Boot DevTools → for live reload during development

3. Click  **Generate** button to download the zip
4. Extract the zip and open in Eclipse or your preferred IDE

Step 3: Configure Database Connection 

1. From the zip file, open application properties from this path src/main/resources/application.properties

2. Add to the file:
    spring.datasource.url=jdbc:postgresql://localhost:5432/cargo_db
    spring.datasource.username=your_username
    spring.datasource.password=your_password
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.show-sql=true

**Update your username and password**

Step 4: Run Application

- In the terminal, run : mvnw spring-boot:run

