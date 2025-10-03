# UserManagementAPI 🚀

This project is a **.NET 6 Web API** for managing users, developed for my coursework.  
It demonstrates CRUD operations, input validation, debugging improvements, and middleware integration.

---

## ✅ Project Rubric Coverage

- **(5 pts) GitHub Repository**  
  This codebase is hosted here: [GitHub Repo Link](https://github.com/Kut1o/UserManagementAPI)

- **(5 pts) CRUD Endpoints**  
  Implemented in `UsersController.cs`:  
  - `GET /api/users` → Retrieve all users  
  - `GET /api/users/{id}` → Retrieve user by ID  
  - `POST /api/users` → Create new user  
  - `PUT /api/users/{id}` → Update existing user  
  - `DELETE /api/users/{id}` → Remove user  

- **(5 pts) Debugging with Copilot**  
  I used Copilot to help debug issues like:  
  - Adding try-catch for unhandled exceptions  
  - Improving validation logic (e.g., regex for email)  
  - Suggesting in-memory repository pattern for thread safety  

- **(5 pts) Input Validation**  
  Users must provide:  
  - **Name** (non-empty)  
  - **Email** (valid format, checked with regex)  

- **(5 pts) Middleware**  
  Implemented and configured in `Program.cs`:  
  - **Error Handling Middleware** → Catches exceptions, returns JSON `{ "error": "Internal server error." }`  
  - **Authentication Middleware** → Requires `Authorization: Bearer secrettoken` header  
  - **Logging Middleware** → Logs HTTP method, path, response status, and request duration  

---

## ⚙️ How to Run

1. Install .NET 6 or later.
2. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/UserManagementAPI.git
   cd UserManagementAPI
