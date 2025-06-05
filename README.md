# Task Manager

A full-stack web application for managing tasks, built with Spring Boot (backend) and React (frontend).

## Features

- Create, read, update, and delete tasks via REST APIs
- Toggle task completion status with checkboxes
- Responsive UI with Tailwind CSS
- H2 in-memory database for task storage
- CORS enabled for frontend-backend integration

## Project Structure

- `backend/`: Spring Boot backend with REST APIs
- `frontend/`: React frontend with task management UI

## Prerequisites

- Java 17 or later
- Maven 3.6 or later
- Node.js 20.x or later
- npm 9.x or later

## Setup Instructions

1. Clone the repository:
   ```bash
   (https://github.com/sharmahiteshwar/task-manager.git)
   ```

2. Backend Setup:
   
   -Navigate to the backend folder: cd backend
   -Install dependencies: mvn clean install
   -Run the backend: mvn spring-boot:run
   -Access the API at http://localhost:8080/api/tasks
   -View the H2 database console at http://localhost:8080/h2-console (JDBC URL: jdbc:h2:mem:testdb, Username: sa, Password: blank)

4. Frontend Setup:
   
   -Open a new terminal and navigate to the frontend folder: cd frontend
   -Install dependencies: npm install
   -Run the frontend: npm start
   -Access the app at http://localhost:3000


Technologies
Backend: Spring Boot, Spring Data JPA, H2 Database, REST
Frontend: React, Tailwind CSS, Axios

Notes
Ensure the backend is running before starting the frontend to avoid CORS errors.
The backend uses an in-memory H2 database, so data resets on restart.
