# expense-tracker-microservices
A full-fledged Expense Tracker built using Spring Boot Microservices, Kafka, Redis, Docker, and AWS basics
### 📘 GitHub README Template: Expense Tracker Microservices

# 💰 Expense Tracker - Microservices Architecture

Track expenses, set budgets, and get real-time alerts when limits are exceeded. Built with Spring Boot, Kafka, Redis, Docker, and deployed to AWS.

---

## 🧱 Architecture Overview

![Architecture](docs/architecture-diagram.png) *(optional to include)*

| Service             | Description                                 |
|---------------------|---------------------------------------------|
| user-service        | Handles user registration & JWT login       |
| transaction-service | Manages income/expense records              |
| budget-service      | Stores and tracks monthly budgets           |
| notification-service| Sends alerts when limits are crossed        |
| api-gateway         | Routes APIs to respective services          |
| config-server       | Centralized config for all microservices    |

---

## ⚙️ Tech Stack
- Java 17+ (can be updated to Java 21)
- Spring Boot 3.x
- Spring Cloud Gateway, Config Server
- JPA + MySQL
- Kafka
- Redis
- Docker & Docker Compose
- GitHub Actions CI/CD
- AWS EC2, S3 (optional)

---

## 🚀 Setup Instructions

```bash
# Prerequisites:
- Java 17 or higher
- Docker & Docker Compose
- MySQL and Redis running (or use Docker Compose)

# Clone the repo
$ git clone https://github.com/yourusername/expense-tracker-microservices.git
$ cd expense-tracker-microservices

# Run all services with Docker Compose
$ docker-compose up --build

# Access Services:
- Gateway: http://localhost:8080
- Swagger Docs: http://localhost:8080/swagger-ui.html
```

---

## ✅ Features
- Secure Login with JWT
- Microservice-to-Microservice Communication
- Async Messaging with Kafka
- Redis-based Budget Cache
- Alert generation when limit exceeds
- CI/CD with GitHub Actions
- Dockerized Setup

---

## 📁 Repository Structure
```plaintext
expense-tracker/
├── user-service/
├── transaction-service/
├── budget-service/
├── notification-service/
├── api-gateway/
├── config-server/
├── docker-compose.yml
└── README.md
```

---

## 📦 Future Enhancements
- Email and SMS Notifications
- PDF Report Generation
- Frontend Dashboard (React/Vue)
- OAuth2 / SSO

---

## 🧪 Test Coverage
Each service includes integration and unit tests with JUnit 5 and Mockito.

---

## ✨ Contributing
Pull requests are welcome. For major changes, please open an issue first.
