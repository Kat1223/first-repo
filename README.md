# 🚀 TaskFlow API

A **production-ready Task Management API** built with **Node.js,
TypeScript, Express, MongoDB, and Socket.IO**.

It demonstrates **clean backend architecture, scalable design, real-time
systems, authentication, and strong testing practices**, making it
suitable for **modern production systems and backend engineering
portfolios**.

------------------------------------------------------------------------

# 🎥 Demo Video

Watch the full project demonstration:

🎬 **Project Demo**\
https://drive.google.com/file/u/1/d/1mNqZPR3IJhIEnS1pz-7cU4BAYV9FDpGW/view?usp=drivesdk

### The demo covers

-   API architecture overview\
-   Authentication workflow\
-   CRUD operations\
-   Real-time socket events\
-   File uploads & exports\
-   Test coverage demonstration

------------------------------------------------------------------------

# 📌 Project Overview

**TaskFlow API** is a modular backend system designed for
**collaborative project and task management**.

### Key Capabilities

✔ Secure JWT authentication\
✔ Project and task collaboration\
✔ Role-based authorization\
✔ Real-time updates via Socket.IO\
✔ File uploads and exports\
✔ High test coverage with Jest\
✔ Production-ready middleware and utilities

Architecture follows:

Controllers → Services → Models → Database

------------------------------------------------------------------------

# ✨ Features

## 🔐 Authentication & Security

-   JWT-based authentication
-   Access & refresh token flow
-   Role-based authorization middleware
-   Secure password hashing

## 📋 Task Management

-   Create, update, and delete tasks
-   Assign tasks to users
-   Task status tracking
-   Comment support

## 📁 Project Management

-   Create projects
-   Manage project members
-   Associate tasks with projects

## 📎 File Handling

-   Task attachments
-   User avatar uploads
-   CSV task exports
-   PDF project reports

## ⚡ Real-Time Features

-   Socket.IO integration
-   Live task status updates
-   Real-time notifications

## 🚀 Performance Features

-   Pagination
-   Cursor-based queries
-   Sorting utilities

## 🏭 Production Utilities

-   Request logging
-   Centralized error handling
-   Rate limiting
-   Compression middleware

## 🧪 Testing

-   Unit tests
-   Integration tests
-   MongoMemoryServer test database
-   80%+ code coverage

------------------------------------------------------------------------

# 🛠 Tech Stack

## Backend

-   Node.js
-   Express.js
-   TypeScript

## Database

-   MongoDB
-   Mongoose

## Real-time

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

  Method   Endpoint            Description
  -------- ------------------- ----------------------
  POST     /api/auth/signup    Register user
  POST     /api/auth/login     Login user
  POST     /api/auth/refresh   Refresh access token
  GET      /api/auth/me        Get current user

## Projects

  Method   Endpoint
  -------- -------------------
  POST     /api/projects
  GET      /api/projects
  GET      /api/projects/:id
  PUT      /api/projects/:id
  DELETE   /api/projects/:id

## Tasks

  Method   Endpoint
  -------- ----------------
  POST     /api/tasks
  GET      /api/tasks
  GET      /api/tasks/:id
  PUT      /api/tasks/:id
  DELETE   /api/tasks/:id

Supports pagination, sorting, and cursor-based queries.

------------------------------------------------------------------------

# ⚙️ Installation

Clone the repository

``` bash
git clone <repository-url>
cd taskflow-api
```

Install dependencies

``` bash
npm install
```

------------------------------------------------------------------------

# 🔑 Environment Variables

Create `.env`

    PORT=3000
    MONGO_URI=your_mongodb_connection
    JWT_SECRET=your_secret
    CORS_ORIGIN=http://localhost:3000

------------------------------------------------------------------------

# ▶️ Running the Application

Development

    npm run dev

Production

    npm run build
    npm start

------------------------------------------------------------------------

# 🧪 Running Tests

Run tests

    npm test

Run with coverage

    npm run test:coverage

------------------------------------------------------------------------

# 📬 Postman Collection

Import:

TaskFlow.postman_collection.json

Includes requests for:

-   Authentication
-   Projects
-   Tasks
-   File uploads

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

**Adhi**\
Backend Developer \| MERN Stack \| Node.js \| TypeScript
