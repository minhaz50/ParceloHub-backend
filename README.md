# [ParceloHub] API

A RESTful backend for managing courier and logistics, with role based access, payments and audit section.

## Live API: https://delivery-backend-n94c.onrender.com/

## Postman Docs: https://documenter.getpostman.com/view/21998234/2sBYB1MTZo

## Frontend :

## Table Of Contents

- Overview
- Features
- Tech Stack
- Roles & Permissions
- Architecture
- Database Schema
- API Overview
- Getting Started
- Environment Variables
- Scripts
- Response Format
- Authentication
- Pagination, Filtering, Sorting & Search
- Payment Flow
- Deployment
- Testing the API
- Project Structure
- Author

---

### Overview

This backend exposes 20+ versioned REST endpoints covering authentication, user management, core resources, business workflows, payments, and admin operations. It uses PostgreSQL with Prisma for relational data, Zod for strict input validation, and role-based middleware to enforce access control.

# **Tech Stack**

| Category             | Technology                      |
| -------------------- | ------------------------------- |
| Runtime & Framework  | Node.js, TypeScript, Express.js |
| Database & ORM       | PostgreSQL, Prisma              |
| Validation           | Zod                             |
| Authentication       | [Custom JWT ] + Google OAuth    |
| File Storage         | Multer, Cloudinary              |
| Payments             | [ Stripe ]                      |
| Linting & Formatting | [Biome / ESLint + Prettier]     |
| Documentation        | Postman                         |
| Deployment           | Render                          |

---

# Roles & Permissions

| Role  | Description            | Key Permission                                                            |
| ----- | ---------------------- | ------------------------------------------------------------------------- |
| ADMIN | Platform administrator | Manage users and roles, view stats, view audit logs, manage all resources |
