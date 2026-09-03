# student-api-DTO-exceptional-handling-filters-wrap-up

A comprehensive Spring Boot REST API for student management with advanced features.

## Features
- **CRUD Operations**: Create, Read, Update, Delete students
- **DTO Pattern**: Data Transfer Objects for clean API contracts
- **Exception Handling**: Centralized exception handling with custom error responses
- **Request Filters**: HTTP request logging filter
- **Validation**: Input validation using Jakarta Validation
- **H2 Database**: In-memory database for testing
- **JPA**: Spring Data JPA for database operations

## Tech Stack
- Spring Boot 3.2.0
- Spring Data JPA
- H2 Database
- Jakarta Validation
- Maven

## Running the Application
```bash
mvn spring-boot:run
```

## API Endpoints
- `GET /api/students` - Get all students
- `GET /api/students/{id}` - Get student by ID
- `POST /api/students` - Create new student
- `PUT /api/students/{id}` - Update student
- `DELETE /api/students/{id}` - Delete student

## H2 Console
Access H2 Console at: http://localhost:8081/h2-console
- JDBC URL: `jdbc:h2:mem:studentdb`
- Username: `sa`
- Password: (empty)

## Project Structure
```
src/main/java/com/example/studentapi/
├── config/          # Configuration classes
├── controller/      # REST controllers
├── dto/            # Data Transfer Objects
├── exception/      # Exception handling
├── filter/         # Servlet filters
├── model/          # Entity models
├── repository/     # JPA repositories
└── service/        # Business logic
```
