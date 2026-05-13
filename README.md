# FamilyBridge — Backend

> REST API for a family coexistence platform designed for children of divorced parents.

## About the project

FamilyBridge helps divorced parents coordinate their children's lives through
a shared calendar, real-time chat, and document management — all synchronized
with Google Calendar.

This project was built as a portfolio piece to demonstrate proficiency in
Java 21, Spring Boot 3, and modern backend architecture.

## Tech stack

- **Language:** Java 21
- **Framework:** Spring Boot 3.3
- **Security:** Spring Security + OAuth2 + JWT
- **Database:** PostgreSQL 16 with Flyway migrations
- **Cache:** Redis 7
- **Integration:** Google Calendar API v3
- **Real-time:** WebSocket with STOMP
- **Storage:** AWS S3
- **Docs:** Springdoc OpenAPI (Swagger UI)
- **Tests:** JUnit 5 + Mockito + Testcontainers

## Architecture

See [docs/architecture.md](docs/architecture.md) for the full architecture overview.

## Running locally

### Prerequisites
- Java 21+
- Docker Desktop

### Steps

```bash
# 1. Clone the repository
git clone https://github.com/SEU_USUARIO/familybridge-backend.git
cd familybridge-backend

# 2. Start dependencies
docker-compose up -d

# 3. Run the application
./mvnw spring-boot:run
```

API available at `http://localhost:8080`
Swagger UI at `http://localhost:8080/swagger-ui.html`

## API overview

| Module | Base path |
|--------|-----------|
| Auth | `/api/v1/auth` |
| Calendar | `/api/v1/calendar` |
| Chat | `/api/v1/chat` |
| Documents | `/api/v1/documents` |
| Users | `/api/v1/users` |

## License

MIT
