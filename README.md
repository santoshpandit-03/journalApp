# Journal App

A production-ready Spring Boot REST API for managing personal journal entries with secure JWT authentication, MongoDB, Redis caching, Kafka messaging, scheduled jobs, email notifications, and weather integration.

## Features

- JWT Authentication & Authorization
- Spring Security
- CRUD Operations for Journal Entries
- MongoDB Database
- Redis Caching
- Apache Kafka Integration
- Email Notifications
- Weather API Integration
- Scheduled Tasks
- RESTful APIs
- SonarQube Code Analysis
- Unit Testing with JUnit & Mockito

## Tech Stack

- Java 17
- Spring Boot 3
- Spring Security
- Spring Data MongoDB
- Redis
- Apache Kafka
- Maven
- JWT
- JUnit 5
- Mockito
- SonarQube
- GitHub Actions

## Project Structure

```
src
├── controller
├── service
├── repository
├── entity
├── filter
├── config
├── scheduler
├── cache
├── constants
├── model
├── enums
└── resources
```

## Environment Variables

Create the following environment variables before running the application.

| Variable | Description |
|----------|-------------|
| MONGODB_URI | MongoDB Connection URI |
| REDIS_URL | Redis Cloud URL |
| MAIL_USERNAME | Gmail Username |
| MAIL_PASSWORD | Gmail App Password |
| KAFKA_BOOTSTRAP_SERVERS | Kafka Bootstrap Servers |
| KAFKA_JAAS_CONFIG | Kafka JAAS Configuration |
| WEATHER_API_KEY | Weather API Key |

## Installation

Clone the repository

```bash
git clone https://github.com/santoshpandit-03/journalApp.git
```

Move into the project

```bash
cd journalApp
```

Build the project

```bash
mvn clean install
```

Run the application

```bash
mvn spring-boot:run
```

## Security

Sensitive information is **not stored** in the repository.

All credentials are loaded securely using Environment Variables and GitHub Secrets.

## CI/CD

GitHub Actions automatically performs:

- Maven Build
- Unit Tests
- SonarQube Analysis

## Testing

Run tests using

```bash
mvn test
```