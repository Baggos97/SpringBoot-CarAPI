# SpringBoot Car Dealership API

A RESTful API for managing a car dealership system, built with Spring Boot 3 and PostgreSQL.

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Java, Spring Boot 3 |
| Database | PostgreSQL |
| ORM | Spring Data JPA / Hibernate |

## Features

- Manage cars, dealerships, citizens and bookings
- Search cars by brand, model, fuel type and max price
- Add cars to a dealership and update stock amounts
- Book a car for a citizen

## Entities

- **Car** — brand, model, fuel type, engine, seats, price, stock amount
- **Dealership** — identified by VAT number, owns cars
- **Citizen** — can make bookings
- **Booking** — links a citizen to a car

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/cars` | Get all cars |
| GET | `/api/cars/search` | Search cars (brand, model, fuel, maxPrice) |
| POST | `/api/addCar` | Add a car to a dealership |
| PUT | `/api/updateCarAmount/{id}` | Update car stock amount |

## How to Run

```bash
# 1. Set up PostgreSQL and update application.properties with your DB credentials

# 2. Run the application
./mvnw spring-boot:run

# API available at http://localhost:8080
```
