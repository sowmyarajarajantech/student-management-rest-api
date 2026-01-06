# Student Management REST API

A RESTful backend application built using Java and Spring Boot to manage student records.  
The project follows clean architecture principles using the Controller–Service–Repository pattern.

---

## Tech Stack

- Java 17
- Spring Boot
- Spring Data JPA (Hibernate)
- H2 Database (development)
- MySQL (production-ready configuration)
- Maven
- Postman

---

## Features

- Create, read, update, and delete student records
- RESTful API design
- Automatic database table creation using Hibernate
- Clean and maintainable layered architecture
- API testing using Postman

---

## Architecture Overview

Controller → Service → Repository → Database

---

## API Endpoints

| Method | Endpoint | Description |
|------|--------|-------------|
| POST | /students | Create a student |
| GET | /students | Retrieve all students |
| GET | /students/{id} | Retrieve student by ID |
| PUT | /students/{id} | Update student |
| DELETE | /students/{id} | Delete student |

---

## Database
- Initially used H2 in-memory database for development
- Migrated to MySQL for persistent storage
- Hibernate auto-creates tables using JPA annotations

---

## Sample Request (Create Student)

```json
{
  "name": "John Doe",
  "email": "john.doe@gmail.com",
  "course": "Java"
}
