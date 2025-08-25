# MarineIT — Backend API (ASP . NET Core)

This repository contains the backend solution for the **Marine IT Service Management (MarineIT)** system. It implements the RESTful API and core business logic for managing service requests, assets, vessels, and maintenance tasks.

---

##  Project Structure

MarineIT/

├── MarineIT.Api/ # ASP.NET Core Web API project (entry point)

├── MarineIT.Application/ # Business logic & services

├── MarineIT.Domain/ # Domain models, entities, enums

├── MarineIT.Infrastructure/ # EF Core, DbContext, repositories

├── MarineIT.sln # Solution file

└── README.md # This file

----


---

##  Features

- **Clean architecture** — separated into Domain, Application, Infrastructure, and API layers.
- **Entity Framework Core** used for data access with a SQL Server provider.
- **Domain-Driven Design** — core models and logic isolated in `Domain` and `Application`.
- **RESTful API** using ASP.NET Core for endpoints.
- **Extensible** — easily scale within DDD patterns or add features like authentication.

---

##  Setup & Run Locally

### Prerequisites:
- .NET 8 SDK (or latest stable)
- SQL Server or LocalDB

---

## API Endpoints (Samples)

- **GET** `/api/vessels` — List all vessels

- **GET** `/api/tickets` — List service tickets

- **POST** `/api/maintenance` — Schedule new maintenance task

- **PUT/PATCH** requests available for updating entities

  ----
## Development Workflow

1. Create new feature branch (`git checkout -b feature/...`).

2. Implement logic in `Application` + `Infrastructure`.

3. Expose or adjust endpoints in `Api` project.

4. Write or update EF migrations if needed.

5. Build and test via `dotnet run` / Swagger.

6. Commit and open a pull request.
  
----
## Roadmap / Next Steps

- Add JWT authentication with role-based access.

- Integrate proper logging and monitoring (Serilog, Health Checks).

- Add caching (e.g. Redis) for performance.

- Dockerize for ease of environment setup.

- Write integration & unit tests for key components.
----


## 🤝 Contributing 

Feel free to fork the repo and submit PRs or raise issues for any suggastions.

--- 

## 📬  Contact
For questions or collaboration opportunities:

**📧 Email:** ali.razi9292@gmail.com

**🔗 LinkedIn:** linkedin.com/in/alirazi1992
