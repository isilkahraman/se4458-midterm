#  Airline Ticketing API (SE4458 Midterm Project)

This project is a RESTful backend API for an airline ticketing system developed using **Java Spring Boot** and **PostgreSQL**. It is built for the **SE4458 Software Engineering** midterm assignment.

---

## Technologies Used

- Java 17  
- Spring Boot 3.4 
- Spring Security (JWT Authentication)  
- PostgreSQL  
- Swagger UI  
- Maven  
- Lombok  

---

## Features

-  JWT-based login
-  Add and query flights
-  Buy ticket
-  Check-in and assign seat
-  Query passenger list with seat info

---

##  Endpoints (Swagger UI)

You can test all endpoints using Swagger:

 [Swagger UI](http://localhost:8081/swagger-ui/index.html)

> Note: First, use `/api/v1/auth/login` to get a JWT token. Then click **"Authorize"** and paste:
>
> ```
> Bearer your.jwt.token
> ```

---

##  Local Setup

### 1. PostgreSQL Setup

Create a PostgreSQL database named:

```sql
CREATE DATABASE airline_db;

Update src/main/resources/application.properties:

spring.datasource.url=jdbc:postgresql://localhost:5432/airline_db
spring.datasource.username=postgres
spring.datasource.password=your_password

Run the App

Access the App
http://localhost:8081/swagger-ui/index.html

Developed by Işıl Kahraman for SE4458 Spring Term 2025 Midterm.




