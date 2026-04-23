# Task Manager API

This is a simple Spring Boot project I built to practice REST API development.

The application allows basic task management operations like creating, updating, deleting, and listing tasks.

## What I implemented

- REST API with Spring Boot  
- Basic CRUD operations  
- Layered structure (Controller → Service → Repository)  
- Exception handling for missing resources  
- Swagger for API testing  

## Tech stack

- Java 17  
- Spring Boot  
- Spring Data JPA  
- H2 Database  
- OpenAPI / Swagger  

## Endpoints

- GET /tasks → list all tasks  
- GET /tasks/{id} → get task by id  
- POST /tasks → create task  
- PUT /tasks/{id} → update task  
- DELETE /tasks/{id} → delete task  

## Running the project

```bash
./mvnw spring-boot:run

Then open:
http://localhost:8080/swagger-ui/index.html

Notes
* I used an in-memory H2 database for simplicity

* Error responses are handled globally (e.g. when task is not found)
Why I built this
I built this project to better understand how Spring Boot works in real-world backend applications, especially the separation of layers and handling API errors.