# 🎧 HelpDesk Management System

A full-stack help desk and ticket management platform built with Next.js, Node.js, TypeScript, PostgreSQL, Prisma, and JWT authentication.

## Project Highlights

* ✅ Full-Stack Architecture (Frontend + Backend)
* ✅ JWT Authentication & Authorization
* ✅ Role-Based Access Control (Admin, Agent, User)
* ✅ PostgreSQL Database with Prisma ORM
* ✅ REST API Architecture
* ✅ Ticket Lifecycle Management
* ✅ Dashboard and Analytics
* ✅ Type-Safe Development with TypeScript

---

## Overview

The HelpDesk Management System is designed to streamline IT support operations by providing a centralized platform for ticket creation, assignment, tracking, and resolution.

The application supports different user roles and permissions, allowing administrators, support agents, and end users to interact with the system according to their responsibilities.

---

## Core Features

### Authentication & Security

* User registration and login
* JWT-based authentication
* Protected routes
* Password hashing with bcrypt
* Role-based access control (RBAC)

### Ticket Management

* Create support tickets
* Update ticket status
* Assign agents to tickets
* Priority management
* Category management
* Ticket history tracking

### User Management

* User registration
* User activation/deactivation
* Role management
* Profile information management

### Dashboard

* Ticket statistics
* Status monitoring
* Operational insights
* Real-time support overview

### Comments & Collaboration

* Ticket comments
* Internal notes
* Communication tracking
* Activity history

---

## Tech Stack

### Frontend

* Next.js 14
* React 18
* TypeScript
* Tailwind CSS
* React Query
* React Hook Form
* Zod
* Axios

### Backend

* Node.js
* Express.js
* TypeScript
* Prisma ORM
* PostgreSQL
* JWT Authentication
* bcryptjs
* Zod Validation

---

## Database Design

### Main Entities

* User
* Ticket
* Comment
* Category
* Ticket History

### User Roles

| Role  | Description                    |
| ----- | ------------------------------ |
| ADMIN | Full system access             |
| AGENT | Ticket handling and resolution |
| USER  | Ticket creation and tracking   |

### Ticket Status

* OPEN
* IN_PROGRESS
* RESOLVED
* CLOSED

### Ticket Priorities

* LOW
* MEDIUM
* HIGH
* CRITICAL

---

## Project Structure

```text
helpdesk-system/
├── backend/
│   ├── prisma/
│   ├── src/
│   │   ├── controllers/
│   │   ├── middlewares/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── repositories/
│   │   ├── config/
│   │   └── utils/
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── lib/
│   │   └── types/
│   └── package.json
│
└── README.md
```

---

## Architecture

### Backend

The backend follows a layered architecture:

* Controllers → Handle HTTP requests
* Services → Business logic
* Repositories → Data access layer
* Middlewares → Authentication and error handling
* Prisma ORM → Database communication

### Frontend

The frontend uses:

* App Router (Next.js 14)
* Reusable UI components
* Custom hooks
* API abstraction layer
* React Query for server-state management

---

## Getting Started

### Clone Repository

```bash
git clone https://github.com/MOISESSILVA22/helpdesk-management-system.git
cd helpdesk-management-system
```

### Backend Setup

```bash
cd backend

npm install

cp .env.example .env

npm run db:generate
npm run db:migrate
npm run db:seed

npm run dev
```

### Frontend Setup

```bash
cd frontend

npm install

cp .env.local.example .env.local

npm run dev
```

---

## Future Improvements

* Email notifications
* File attachments
* WebSocket real-time updates
* Audit logs
* Docker containerization
* CI/CD pipeline
* Automated testing
* Multi-tenant architecture

---

## Author

**Francisco Moisés Silva da Luz**

**Back-end Developer | Systems Analysis and Development Student**

GitHub:
https://github.com/MOISESSILVA22

LinkedIn:
https://linkedin.com/in/moisés-silvaa
