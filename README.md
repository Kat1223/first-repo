# 🚀 TaskFlow API

```{=html}
<p align="center">
```
![Node.js](https://img.shields.io/badge/Node.js-18+-green?style=for-the-badge&logo=node.js)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?style=for-the-badge&logo=typescript)
![Express](https://img.shields.io/badge/Express.js-Backend-black?style=for-the-badge&logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?style=for-the-badge&logo=mongodb)
![Socket.IO](https://img.shields.io/badge/Socket.IO-Realtime-orange?style=for-the-badge&logo=socket.io)
![Jest](https://img.shields.io/badge/Tested%20With-Jest-red?style=for-the-badge&logo=jest)

```{=html}
</p>
```
A **production-ready Task Management API** built with:

**Node.js • TypeScript • Express • MongoDB • Socket.IO**

This project demonstrates **clean backend architecture, scalable API
design, real-time systems, authentication, and strong testing
practices**, making it suitable for **modern production systems and
backend engineering portfolios**.

------------------------------------------------------------------------

# 🎥 Demo Video

Watch the full project demonstration.

🎬 **Project Demo**

https://drive.google.com/file/u/1/d/1mNqZPR3IJhIEnS1pz-7cU4BAYV9FDpGW/view?usp=drivesdk

### The demo covers

• Backend architecture overview\
• Authentication workflow\
• Task & project CRUD APIs\
• Real-time Socket.IO events\
• File uploads and exports\
• Automated testing and coverage

------------------------------------------------------------------------

# 📌 Project Overview

**TaskFlow API** is a modular backend system designed for
**collaborative task and project management**.

It includes:

✔ Secure authentication\
✔ Real-time updates\
✔ File handling\
✔ Scalable architecture\
✔ Production middleware\
✔ High test coverage

### Architecture Pattern

Controllers → Services → Models → Database

------------------------------------------------------------------------

# ✨ Features

## 🔐 Authentication & Security

-   JWT based authentication
-   Access token & refresh token flow
-   Role based authorization
-   Secure password hashing
-   Protected routes middleware

## 📋 Task Management

-   Create tasks
-   Update tasks
-   Delete tasks
-   Assign tasks to users
-   Track task status
-   Task comments

## 📁 Project Management

-   Create projects
-   Add project members
-   Manage project roles
-   Associate tasks with projects

## 📎 File Handling

-   Task attachments
-   User avatar uploads
-   CSV task export
-   PDF project reports

## ⚡ Real-Time Features

-   Socket.IO integration
-   Live task status updates
-   Real-time notifications
-   Room-based project communication

## 🚀 Performance Features

-   Pagination support
-   Cursor based queries
-   Sorting utilities
-   Optimized database queries

## 🏭 Production Utilities

-   Centralized error handling
-   Request logging
-   Rate limiting
-   Compression middleware
-   Environment configuration

## 🧪 Testing

-   Unit tests
-   Integration tests
-   MongoMemoryServer database
-   API testing with Supertest
-   High code coverage

------------------------------------------------------------------------

# 🛠 Tech Stack

## Backend

-   Node.js
-   Express.js
-   TypeScript

## Database

-   MongoDB
-   Mongoose

## Realtime Communication

-   Socket.IO

## Testing

-   Jest
-   Supertest
-   MongoMemoryServer

## Utilities

-   Multer
-   jsonwebtoken
-   express-validator

------------------------------------------------------------------------

# 🏗 Project Architecture

    src
    │   app.ts
    │   server.ts
    │
    ├── config
    │   config.ts
    │   multer.config.ts
    │
    ├── controllers
    │   auth.controller.ts
    │   project.controller.ts
    │   task.controller.ts
    │   comment.controller.ts
    │   attachment.controller.ts
    │   avatar.controller.ts
    │   health.controller.ts
    │
    ├── middleware
    │   auth.middleware.ts
    │   error.middleware.ts
    │   role.middleware.ts
    │   socket.middleware.ts
    │   production.middleware.ts
    │
    ├── models
    │   user.model.ts
    │   project.model.ts
    │   task.model.ts
    │   comment.model.ts
    │
    ├── routes
    │   auth.routes.ts
    │   project.routes.ts
    │   task.routes.ts
    │   health.routes.ts
    │
    ├── services
    │   auth.service.ts
    │   project.service.ts
    │   task.service.ts
    │   socket.service.ts
    │   email.service.ts
    │
    ├── utils
    │   logger.util.ts
    │   token.util.ts
    │   pagination.util.ts
    │   cursor.util.ts
    │   sort.util.ts
    │   appError.ts
    │
    └── validators
        task.validator.ts

------------------------------------------------------------------------

# 🌐 API Endpoints

## Authentication

  Method   Endpoint              Description
  -------- --------------------- ----------------------
  POST     `/api/auth/signup`    Register user
  POST     `/api/auth/login`     Login user
  POST     `/api/auth/refresh`   Refresh access token
  GET      `/api/auth/me`        Get current user

## Projects

  Method   Endpoint              Description
  -------- --------------------- ------------------
  POST     `/api/projects`       Create project
  GET      `/api/projects`       Get all projects
  GET      `/api/projects/:id`   Get project
  PUT      `/api/projects/:id`   Update project
  DELETE   `/api/projects/:id`   Delete project

## Tasks

  Method   Endpoint           Description
  -------- ------------------ -------------
  POST     `/api/tasks`       Create task
  GET      `/api/tasks`       Get tasks
  GET      `/api/tasks/:id`   Get task
  PUT      `/api/tasks/:id`   Update task
  DELETE   `/api/tasks/:id`   Delete task

Supports:

• Pagination\
• Sorting\
• Cursor based queries

------------------------------------------------------------------------

# ⚙️ Installation

### Clone repository

``` bash
git clone <repository-url>
cd taskflow-api
```

### Install dependencies

``` bash
npm install
```

------------------------------------------------------------------------

# 🔑 Environment Variables

Create a `.env` file.

    PORT=3000
    MONGO_URI=your_mongodb_connection
    JWT_SECRET=your_secret_key
    CORS_ORIGIN=http://localhost:3000

------------------------------------------------------------------------

# ▶️ Running the Application

### Development

    npm run dev

### Production

    npm run build
    npm start

------------------------------------------------------------------------

# 🧪 Running Tests

Run all tests

    npm test

Run with coverage

    npm run test:coverage

------------------------------------------------------------------------

# 📬 Postman Collection

Import the collection:

    TaskFlow.postman_collection.json

Includes requests for:

• Authentication\
• Projects\
• Tasks\
• File uploads

------------------------------------------------------------------------

# 🏷 Version Tags

    v0.1.0-foundation
    v0.2.0-models
    v0.3.0-crud-api
    v0.4.0-auth-system
    v0.5.0-validation-error-handling
    v0.6.0-file-handling
    v0.7.0-realtime-pagination
    v0.8.0-production-email
    v1.0.0-taskflow-api

------------------------------------------------------------------------

# 👨‍💻 Author

**Adhi**

Backend Developer\
MERN Stack \| Node.js \| TypeScript
