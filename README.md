# 🚀 TaskFlow API

![Node.js](https://img.shields.io/badge/Node.js-18+-green)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-green)
![Coverage](https://img.shields.io/badge/Test%20Coverage-80%25+-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

TaskFlow API is a **production-ready task management backend** built
with **Node.js, Express, TypeScript, MongoDB Atlas, and Socket.io**.

It supports authentication, project and task management, file uploads,
real-time updates, email notifications, and advanced query utilities.

------------------------------------------------------------------------

# 📌 Features

### 🔐 Authentication

-   JWT Access + Refresh tokens
-   Secure password hashing (bcrypt)
-   Password reset via email
-   Protected routes

### 👤 User Management

-   Signup & login
-   Get current user
-   Avatar upload

### 📁 Project Management

-   Create projects
-   Assign members
-   Project activity tracking

### ✅ Task Management

-   Create and update tasks
-   Task assignment
-   Priority and status management
-   Soft delete tasks

### 💬 Comments

-   Add comments to tasks
-   Track task discussions

### 📎 Attachments

-   Upload files
-   Download attachments

### ⚡ Real-Time Updates

Using **Socket.io** - Task updates - Comment notifications - Project
events

### 📊 Query Utilities

-   Pagination
-   Sorting
-   Filtering
-   Cursor pagination

### 📧 Email Notifications

Using **Nodemailer** - Welcome email - Password reset email - Task
assignment notifications - Comment alerts

### 🛡 Security

-   Helmet
-   Rate limiting
-   Input validation
-   Global error handling

------------------------------------------------------------------------

# 🛠 Tech Stack

## Backend

-   Node.js
-   Express.js
-   TypeScript

## Database

-   MongoDB Atlas
-   Mongoose

## Realtime

-   Socket.io

## Authentication

-   JWT
-   bcrypt

## File Upload

-   Multer

## Email

-   Nodemailer

## Testing

-   Jest
-   Supertest
-   MongoMemoryServer

------------------------------------------------------------------------

# 📂 Project Structure

    src
    │
    ├── config
    │   └── multer.config.ts
    │
    ├── controllers
    │   ├── auth.controller.ts
    │   ├── project.controller.ts
    │   ├── task.controller.ts
    │   └── comment.controller.ts
    │
    ├── middleware
    │   ├── auth.middleware.ts
    │   ├── error.middleware.ts
    │   ├── role.middleware.ts
    │   └── socket.middleware.ts
    │
    ├── models
    │   ├── user.model.ts
    │   ├── project.model.ts
    │   ├── task.model.ts
    │   └── comment.model.ts
    │
    ├── routes
    │   ├── auth.routes.ts
    │   ├── project.routes.ts
    │   ├── task.routes.ts
    │   └── health.routes.ts
    │
    ├── services
    │   ├── auth.service.ts
    │   ├── project.service.ts
    │   ├── task.service.ts
    │   ├── email.service.ts
    │   └── socket.service.ts
    │
    ├── utils
    │   ├── logger.util.ts
    │   ├── pagination.util.ts
    │   ├── sort.util.ts
    │   └── token.util.ts
    │
    ├── validators
    │   └── task.validator.ts
    │
    ├── app.ts
    └── server.ts

------------------------------------------------------------------------

# ⚙️ Environment Variables

Create a `.env` file in the root directory.

    PORT=3000
    MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/taskflow
    JWT_SECRET=supersecret
    CORS_ORIGIN=http://localhost:3000

    EMAIL_HOST=smtp.ethereal.email
    EMAIL_PORT=587
    EMAIL_USER=email@example.com
    EMAIL_PASSWORD=password
    EMAIL_FROM="TaskFlow API <noreply@taskflow.com>"

------------------------------------------------------------------------

# 🚀 Installation

Clone the repository

    git clone https://github.com/yourusername/taskflow-api.git
    cd taskflow-api

Install dependencies

    npm install

Run development server

    npm run dev

Server runs on:

    http://localhost:3000

------------------------------------------------------------------------

# 🧪 Running Tests

Run tests

    npm test

Run coverage

    npm run test:coverage

------------------------------------------------------------------------

# 📡 API Endpoints

## Authentication

### Signup

POST /api/auth/signup

Example body

``` json
{
  "email": "user@test.com",
  "password": "password123",
  "name": "User"
}
```

### Login

POST /api/auth/login

### Refresh Token

POST /api/auth/refresh

### Current User

GET /api/auth/me

Header

Authorization: Bearer `<token>`{=html}

------------------------------------------------------------------------

# 📁 Project Routes

Create project

POST /api/projects

Get projects

GET /api/projects

------------------------------------------------------------------------

# ✅ Task Routes

Create task

POST /api/tasks

Get tasks

GET /api/tasks

Update task

PUT /api/tasks/:id

Delete task

DELETE /api/tasks/:id

------------------------------------------------------------------------

# ⚡ Real-time Events

Socket.io events

-   task:created
-   task:updated
-   comment:added
-   project:updated

------------------------------------------------------------------------

# 👨‍💻 Author

Adhi\
Backend Developer \| Node.js \| MongoDB \| TypeScript
