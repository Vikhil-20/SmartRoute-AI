# Backend Architecture

The backend follows a layered architecture.

Presentation Layer

↓

Controller Layer

↓

Service Layer

↓

Repository Layer

↓

Database

Each layer has a single responsibility.

Controllers

- Receive HTTP Requests

Services

- Business Logic

Repositories

- Database Access

Database

- PostgreSQL

Cache

- Redis

Authentication

- JWT