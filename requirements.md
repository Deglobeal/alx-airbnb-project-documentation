# Backend Requirement Specifications - Airbnb Clone

This document defines the functional and technical requirements for three key backend features:  
1. User Authentication  
2. Property Management  
3. Booking System

---

## 1. User Authentication

### 🔧 Functional Requirements
- Users can register with an email and password.
- Users can log in and receive a JWT token.
- Users can log out (client-side token deletion).
- OAuth support (Google) for social login.

### 🔌 API Endpoints

| Method | Endpoint        | Description          |
|--------|------------------|----------------------|
| POST   | /api/register/   | Register a new user  |
| POST   | /api/login/      | Authenticate user and return JWT |
| POST   | /api/logout/     | Log out user (token deletion) |

### 🔎 Input/Output

#### ✅ Register:
**Input (JSON):**
```json
{
  "email": "user@example.com",
  "password": "securePassword123"
}
