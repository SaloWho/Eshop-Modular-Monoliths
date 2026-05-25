# Eshop Modular Monoliths

A learning project for building an e-commerce application using a modular monolith architecture with .NET.

## Project Goal

The goal of this project is to practise building a clean, maintainable e-commerce system where the application is divided into feature-based modules instead of separate microservices.

Each module should have clear boundaries, its own business logic, and its own data access area while still running inside one deployable application.

## Architecture Approach

This project is planned as a **Modular Monolith** using **Vertical Slice Architecture**.

Instead of splitting the system into many separately deployed services from the beginning, the application will be organised into independent modules inside one solution.

This keeps development simpler while still preparing the project for future growth.

## Planned Modules

- **Catalog Module** - manages products, categories, and product details.
- **Basket Module** - manages customer shopping baskets.
- **Ordering Module** - handles checkout, orders, and order history.
- **Payment Module** - payment integration placeholder for future implementation.
- **Identity Module** - authentication and authorization.
- **Shared Kernel** - common abstractions and shared building blocks used carefully across modules.

## Planned Technologies

- .NET / ASP.NET Core Web API
- PostgreSQL
- Entity Framework Core
- Redis
- RabbitMQ
- MassTransit
- Docker
- Keycloak / OpenID Connect
- CQRS
- MediatR
- Carter / Minimal APIs
- Vertical Slice Architecture
- Domain-Driven Design concepts
- Outbox Pattern

## Suggested Solution Structure

```text
src/
  Eshop.Api/
  Eshop.Modules.Catalog/
  Eshop.Modules.Basket/
  Eshop.Modules.Ordering/
  Eshop.Modules.Payment/
  Eshop.Modules.Identity/
  Eshop.SharedKernel/
tests/
  Eshop.Tests/
