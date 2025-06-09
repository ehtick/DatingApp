# DatingApp

A full-stack web application built with ASP.NET Core Web API and Angular, designed to simulate a modern dating platform with real-time messaging, authentication, and responsive UI.

---

## Tech Stack

### Backend
- ASP.NET Core 8 (Web API)
- Entity Framework Core
- AutoMapper
- SignalR (real-time messaging)
- JWT Authentication
- SQLite (dev) / PostgreSQL or SQL Server (prod-ready)

### Frontend
- Angular 17
- RxJS
- Bootstrap & ngx-bootstrap
- Angular Forms & HTTP Interceptors

---

## Features

-  User Registration & Login with JWT
- Photo Upload via Cloudinary
- User Profile Management
- Like/Unlike Functionality
- Real-Time Messaging with SignalR
- Pagination, Filtering, and Sorting
- Authentication Guards & Resolvers
- Responsive Design (Mobile-Friendly)

---

To run the project locally,
### Prerequisites

- [.NET 8 SDK]
- [Node.js]
- Angular CLI 
- SQLite tools

Step 1: Backend Setup


cd API
dotnet restore
dotnet ef database update
dotnet run

Step 2: Frontend Setup

cd client
npm install
ng serve

### Folder Structure Overview:
DatingApp/
├── API/            # .NET Core Web API project
│   ├── Controllers/
│   ├── Data/
│   ├── Entities/
│   ├── Middleware/
│   ├── SignalR/
│   └── appsettings.json
├── client/         # Angular frontend
│   └── src/
├── docker-compose.yml
├── README.md
└── .gitignore


### Docker Support

version: '3.8'

services:
  sql:
    image: mcr.microsoft.com/azure-sql-edge:latest
    container_name: datingapp_sql
    restart: unless-stopped
    environment:
      ACCEPT_EULA: "1"
      MSSQL_SA_PASSWORD: "${MSSQL_SA_PASSWORD:-StrongP@ssw0rd123}"
    ports:
      - "1433:1433"
    volumes:
      - sql_data:/var/opt/mssql
    healthcheck:
      test: ["CMD", "sqlcmd", "-U", "sa", "-P", "${MSSQL_SA_PASSWORD:-StrongP@ssw0rd123}", "-Q", "SELECT 1"]
      interval: 30s
      timeout: 10s
      retries: 5

volumes:
  sql_data:


### Future Improvements 

Push Notifications                      

Multi-language Support 
