# Airline Ticketing System API - SE4458 Midterm Project

This is a RESTful API developed for SE4458 Software Engineering course, implementing a basic airline ticketing system using **Java Spring Boot**, **PostgreSQL**, and **JWT authentication**.

---

## Technologies Used

- Java 17
- Spring Boot 3.4.4
- Spring Security + JWT
- PostgreSQL (local setup)
- Swagger UI (API testing)
- Maven
- Lombok

---

## Features

| Function | Endpoint | Access |
|---------|----------|--------|
| Login and receive token | `POST /api/v1/auth/login` | Public |
| Add a new flight | `POST /api/v1/flights` | Requires JWT |
| Query available flights | `GET /api/v1/flights` | Public |
| Buy ticket for flight | `POST /api/v1/tickets` | Requires JWT |
| Check-in and assign seat | `POST /api/v1/checkin` | Public |
| List passengers by flight | `GET /api/v1/passengers` | Requires JWT |

---

## Authentication

Use the login endpoint to get a token:

