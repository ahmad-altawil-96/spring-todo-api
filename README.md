# Task Manager API

A simple REST API for managing tasks, built to practice Spring Boot and Java backend development.

## Tech Stack

- Java 21
- Spring Boot 4.0.5
- Spring Security + JWT
- PostgreSQL
- Lombok

## Features

- User registration and login with JWT authentication
- Create, read, update, and delete tasks
- Input validation and error handling

## Getting Started

### Prerequisites
- Java 21
- PostgreSQL
- Maven

### Installation

1. Clone the repository
   git clone https://github.com/USERNAME/spring-todo-api.git

2. Create a PostgreSQL database
   CREATE DATABASE todo_db;

3. Add your configuration in application.properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/todo_db
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   jwt.secret=your_secret_key

4. Run the project
   mvn spring-boot:run

## API Endpoints

### Auth
- POST /auth/register — Register a new user
- POST /auth/login — Login and get JWT token

### Tasks (require JWT token)
- GET /tasks — Get all tasks
- GET /tasks/{id} — Get task by ID
- POST /tasks — Create a new task
- PUT /tasks/{id} — Update a task
- DELETE /tasks/{id} — Delete a task

## Purpose

This project was built as a learning exercise to practice Spring Boot, REST API design, and JWT authentication.
