# Employee Management System

A full-stack Employee Management System built with Angular, Spring Boot, Spring Data JPA, and MySQL. The application allows users to manage employee records through a clean web interface backed by RESTful APIs.

## Project Highlights

- Developed an end-to-end CRUD application for employee record management.
- Built a responsive Angular frontend with list, create, update, delete, and employee detail views.
- Created REST APIs using Spring Boot for employee operations.
- Integrated Angular services with backend APIs using HttpClient and Observables.
- Persisted employee data in MySQL using Spring Data JPA and Hibernate.
- Configured CORS to enable smooth frontend-backend communication during local development.

## Tech Stack

### Frontend

- Angular
- TypeScript
- HTML
- CSS
- Bootstrap
- RxJS

### Backend

- Java
- Spring Boot
- Spring Web MVC
- Spring Data JPA
- Hibernate
- MySQL

## Features

- View all employees in a structured table.
- Add a new employee with first name, last name, and email.
- View complete details of a selected employee.
- Update existing employee information.
- Delete employee records.
- REST API based communication between frontend and backend.
- MySQL database integration for persistent storage.

## Project Structure

```text
EmployeeManagementSystem/
+-- angular-frontend/      # Angular frontend application
`-- springboot-backend/    # Spring Boot backend application
```

## API Endpoints

Base URL:

```text
http://localhost:8080/api/v1
```

| Method | Endpoint | Description |
| --- | --- | --- |
| GET | `/employees` | Get all employees |
| POST | `/employees` | Create a new employee |
| GET | `/employees/{id}` | Get employee by ID |
| PUT | `/employees/{id}` | Update employee by ID |
| DELETE | `/employees/{id}` | Delete employee by ID |

## Prerequisites

Make sure the following tools are installed:

- Java 21 or compatible version
- Maven
- Node.js
- npm
- Angular CLI
- MySQL Server

## Database Setup

Create a MySQL database:

```sql
CREATE DATABASE employee_management_system;
```

Update the database credentials in:

```text
springboot-backend/src/main/resources/application.properties
```

Example:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/employee_management_system?allowPublicKeyRetrieval=true&useSSL=false
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
```

## Backend Setup

Go to the backend folder:

```bash
cd springboot-backend
```

Run the Spring Boot application:

```bash
mvn spring-boot:run
```

The backend will start at:

```text
http://localhost:8080
```

## Frontend Setup

Go to the frontend folder:

```bash
cd angular-frontend
```

Install dependencies:

```bash
npm install
```

Run the Angular development server:

```bash
npm start
```

The frontend will start at:

```text
http://localhost:4200
```

## How It Works

1. The Angular frontend sends HTTP requests to the Spring Boot backend.
2. The backend exposes REST endpoints for employee CRUD operations.
3. Spring Data JPA communicates with MySQL to store and retrieve employee data.
4. The frontend updates the UI based on API responses.

## Key Learnings

- Building full-stack applications using Angular and Spring Boot.
- Designing REST APIs and consuming them from a frontend client.
- Connecting Java applications with MySQL using Spring Data JPA.
- Managing frontend routing, forms, services, and component-based UI.
- Handling cross-origin communication between frontend and backend.

## Author

**Sagar Paul**

- GitHub: [sagarpaul9475](https://github.com/sagarpaul9475)
- LinkedIn: [sagar-paul-2b620928b](https://linkedin.com/in/sagar-paul-2b620928b)
