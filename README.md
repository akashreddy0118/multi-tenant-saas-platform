#  Multi-Tenant SaaS Platform

A scalable **Software as a Service (SaaS)** web application that enables multiple organizations (tenants) to manage their projects, users, and data within a single platform while ensuring secure data isolation.

---

##  Features

*  JWT-based Authentication & Authorization (Admin/User roles)
*  Multi-Tenant Architecture (tenant-based data isolation)
*  Project & Task Management
*  Subscription-based Feature Gating (Free vs Premium)
*  RESTful API Design with validation & pagination
*  Dashboard UI for tenant-specific data

---

##  Tech Stack

### Backend

* Java
* Spring Boot
* REST APIs
* JWT Authentication

### Frontend

* React
* JavaScript
* Axios

### Database

* PostgreSQL

---

##  Architecture Overview

* Backend services built with Spring Boot
* REST APIs for communication between frontend and backend
* PostgreSQL for relational data storage
* Tenant isolation using tenant_id (or schema-based approach)
* React frontend for dashboard and user interaction

---

##  Project Structure

```
backend/    # Spring Boot backend
frontend/   # React frontend
database/   # SQL schema and scripts
docs/       # Architecture and design docs
```

---

##  Setup Instructions

### 1. Clone the repository

```
git clone https://github.com/akashreddy0118/multi-tenant-saas-platform.git
cd multi-tenant-saas-platform
```

### 2. Backend Setup

```
cd backend
./mvnw spring-boot:run
```

### 3. Frontend Setup

```
cd frontend
npm install
npm start
```

### 4. Database Setup

* Install PostgreSQL
* Create database: `saas_db`
* Run schema.sql from `/database`

---

##  Authentication Flow

* User logs in → receives JWT token
* Token is sent in headers for API requests
* Backend validates token and enforces role-based access

---

##  Future Improvements

* Redis caching for performance
* Docker & containerization
* CI/CD pipeline
* Async job processing (Kafka/RabbitMQ)

---

##  Author

Akash Kumar Reddy Pallerla

---
