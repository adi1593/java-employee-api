# Java End-to-End Employee Management REST API

A beginner/interview-friendly end-to-end Java backend project using:
- Java 17
- Spring Boot
- Spring Web / REST
- Spring Data JPA
- H2 database
- Bean Validation
- Global exception handling
- Maven

## Run

Prerequisites:
1. JDK 17+
2. Maven 3.9+

From the project folder:

```bash
mvn clean test
mvn spring-boot:run
```

API base URL:
`http://localhost:8080/api/employees`

## APIs

GET all:
`GET /api/employees`

Filter:
`GET /api/employees?department=IT`

GET one:
`GET /api/employees/1`

POST:
```json
{
  "name": "Rahul Verma",
  "email": "rahul@example.com",
  "department": "Cloud",
  "salary": 70000
}
```

PUT:
`PUT /api/employees/1`

```json
{
  "name": "Rahul Updated",
  "email": "rahul.updated@example.com",
  "department": "AWS",
  "salary": 80000
}
```

DELETE:
`DELETE /api/employees/1`

## H2 Console

URL: `http://localhost:8080/h2-console`

JDBC URL:
`jdbc:h2:file:./data/employeedb`

Username: `sa`
Password: empty

## Suggested next production upgrades

- MySQL/Amazon RDS
- Spring Security + JWT
- Docker
- AWS EC2 deployment
- Application Load Balancer
- Auto Scaling
- CloudWatch monitoring
- Route 53
- CI/CD with GitHub Actions
