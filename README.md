
# TaskFlow API

A production-ready Node.js Task Management API built with **TypeScript, Express, MongoDB, and Socket.IO**, featuring authentication, role-based access control, file handling, real-time updates, and comprehensive testing.

This project demonstrates **clean architecture, scalable backend design, and robust testing practices** suitable for modern production systems.

---

# Demo Video

Watch the full project demonstration:

Demo:  
https://drive.google.com/file/u/1/d/1mNqZPR3IJhIEnS1pz-7cU4BAYV9FDpGW/view?usp=drivesdk

---

# Project Overview

TaskFlow API is a modular backend system designed for managing projects and tasks collaboratively.

It provides:

- Secure JWT authentication
- Project & task management
- Role-based authorization
- Real-time task updates
- File uploads and exports
- Comprehensive testing with Jest
- Production-ready architecture

---

# Features

## Authentication & Security
- JWT-based authentication
- Access & refresh token flow
- Role-based authorization middleware
- Secure password hashing

## Task Management
- Create, update, delete tasks
- Task assignment
- Task status tracking
- Comment support

## Project Management
- Create projects
- Manage project members
- Associate tasks with projects

## File Handling
- Task attachments
- Avatar uploads
- CSV task exports
- PDF project reports

## Real-Time Features
- Socket.IO real-time updates
- Live task status updates
- Real-time notifications

## Performance Features
- Pagination
- Cursor-based queries
- Sorting utilities

## Production Utilities
- Request logging
- Error handling system
- Rate limiting
- Compression middleware

## Testing
- Unit tests
- Integration tests
- MongoMemoryServer test database
- >80% code coverage

---

# Tech Stack

Backend
- Node.js
- Express.js
- TypeScript

Database
- MongoDB
- Mongoose

Real-time
- Socket.IO

Testing
- Jest
- Supertest
- MongoMemoryServer

Utilities
- Multer
- jsonwebtoken
- express-validator

---

# Project Architecture

Controllers → Services → Models → Database

---

# Installation

Clone the repository:

git clone <repository-url>
cd taskflow-api

Install dependencies:

npm install

---

# Environment Variables

Create a `.env` file:

PORT=3000  
MONGO_URI=your_mongodb_connection  
JWT_SECRET=your_secret  
CORS_ORIGIN=http://localhost:3000  

---

# Running the Application

Development mode:

npm run dev

Production:

npm run build  
npm start

---

# Running Tests

npm test

Coverage:

npm run test:coverage

---

# Postman Collection

The repository includes a **Postman collection** for testing all API endpoints.

Import:

TaskFlow.postman_collection.json

---

# Version Tags

v0.1.0-foundation  
v0.2.0-models  
v0.3.0-crud-api  
v0.4.0-auth-system  
v0.5.0-validation-error-handling  
v0.6.0-file-handling  
v0.7.0-realtime-pagination  
v0.8.0-production-email  
v1.0.0-taskflow-api  

---

# Author

Adhi

---

# License

This project was developed as part of a backend engineering exercise.
