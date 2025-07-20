# 🍇 WEEK 5: ASP.NET Core 8.0 Web API & Microservices - Hands-On Implementation

👩‍💻 **Author:** Ananya Upadhyay (6364141)  
📅 **Week:** 5  
🛠️ **Technologies:** ASP.NET Core 8.0, Web API, JWT, Microservices Architecture

---

## 🚀 Project 1: `WebApi_Handson` – FruitsController6

### 📂 Controller: `FruitsController6.cs`

A simple yet powerful API that allows you to interact with a list of fruits.  

### 🔧 Features:

- **GET all fruits** with optional:
  - `sort` (`asc` / `desc`)
  - `page` and `pageSize` for pagination
- **Search** fruits by partial name match: `/search?name=...`
- **Error testing endpoint**: `/throw` – throws an exception to test global error handling

### ✅ Example Endpoints:

GET /api/FruitsController6
GET /api/FruitsController6?sort=desc&page=1&pageSize=3
GET /api/FruitsController6/search?name=man
GET /api/FruitsController6/throw

yaml
Copy
Edit

---

## 🧱 Project 2: Microservices JWT Authentication API

A secured microservice built with **JWT Auth**, designed using ASP.NET Core Web API.

### 📂 Files Overview:

- `AuthController.cs`: Handles login and JWT generation
- `SecureController.cs`: A protected endpoint requiring valid JWT
- `UserModel.cs`: Model for login credentials
- `Program.cs`: Startup and JWT config
- `appsettings.json`: JWT secrets and issuer/audience

---

## 🔐 Authentication Flow

### 1. 🔑 Login

POST /api/Auth/login

css
Copy
Edit

#### Body:
```json
{
  "username": "admin",
  "password": "admin"
}
Returns:

json
Copy
Edit
{
  "token": "<JWT_TOKEN>"
}
2. 🔒 Access Secure Endpoint
bash
Copy
Edit
GET /api/Secure/data
Header:

makefile
Copy
Edit
Authorization: Bearer <JWT_TOKEN>
Returns:

kotlin
Copy
Edit
Hello <user>, this is protected data only visible with a valid token.
📸 Screenshots
Screenshots are embedded in the original .docx for visual reference. They demonstrate successful API execution via Swagger and Postman.

🛠 Setup Instructions
Clone or download the repo.

Make sure you have .NET SDK 8.0+ installed.

Run:

bash
Copy
Edit
dotnet restore
dotnet build
dotnet run
Use Swagger or Postman to test endpoints.

💡 Notes
Ensure appsettings.json contains the correct JWT configuration.

Use Swagger UI to test Bearer token functionality.

Exception handling demo via /throw helps test global error middleware setup.

✨ Extras
🌈 Screenshots + code walkthrough included in the original .docx
📁 All controllers are modular and scalable
🔐 JWT is symmetric key-based with 60-min expiry


