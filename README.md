# Microservices Application (.NET + DDD + CQRS)
Microservices application built with .NET, C#, DDD, and CQRS — featuring Users (PostgreSQL), Products (MongoDB), and Orders (SQL Server) services.

This repository contains a microservices-based application built using:

- ✅ .NET (latest)
- ✅ C# and ASP.NET Core
- ✅ Domain-Driven Design (DDD)
- ✅ CQRS Pattern (via MediatR)
- ✅ PostgreSQL, MongoDB, and SQL Server
- ✅ Serilog, AutoMapper, FluentValidation
- ✅ API Gateway (Ocelot/YARP)
- ✅ Docker-ready (optional)

## 🧱 Microservices Overview

| Service   | Tech Stack                       | Database     |
|-----------|----------------------------------|--------------|
| Users     | .NET + EF Core + MediatR         | PostgreSQL   |
| Products  | .NET + MongoDB Driver + CQRS     | MongoDB      |
| Orders    | .NET + Dapper + CQRS             | SQL Server   |

## 🗂 Project Structure

ncs-microservices/
│
├── .gitignore
├── README.md
├── docker-compose.yml         # (Optional: for local orchestration)
├── gateway/                   # API Gateway (e.g., Ocelot/YARP)
│
├── services/
│   ├── users/                 # Users microservice
│   │   ├── Users.Api/
│   │   ├── Users.Application/
│   │   ├── Users.Domain/
│   │   ├── Users.Infrastructure/
│   │   └── Users.Contracts/
│   │
│   ├── products/              # Products microservice
│   │   ├── Products.Api/
│   │   ├── Products.Application/
│   │   ├── Products.Domain/
│   │   ├── Products.Infrastructure/
│   │   └── Products.Contracts/
│   │
│   └── orders/                # Orders microservice
│       ├── Orders.Api/
│       ├── Orders.Application/
│       ├── Orders.Domain/
│       ├── Orders.Infrastructure/
│       └── Orders.Contracts/
│
└── shared/                    # Optional shared libraries (if any)
