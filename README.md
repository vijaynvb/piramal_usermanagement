# User Management Spring Boot Application

This project is a Spring Boot application that provides a RESTful API for managing users. It uses in-memory storage for user data and includes the following features:

- User model: name, email, password
- CRUD REST API endpoints with versioning: `/api/v1/users`
- Spring Boot Actuator for health and metrics endpoints
- In-memory database for testing

## Getting Started

### Prerequisites
- Java 17 or later
- Maven

### Running the Application

```
./mvnw spring-boot:run
```

The application will start on `http://localhost:8080`.

### API Endpoints
- `POST /api/v1/users` - Create a new user
- `GET /api/v1/users` - Get all users
- `GET /api/v1/users/{id}` - Get user by ID
- `PUT /api/v1/users/{id}` - Update user
- `DELETE /api/v1/users/{id}` - Delete user

### Actuator Endpoints
- `/actuator/health`
- `/actuator/metrics`

### Running Tests

```
./mvnw test
```

## License

This project is licensed under the MIT License.
