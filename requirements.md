# 🏡 Airbnb Clone Backend – Requirements

##  Objective
Document the technical and functional requirements for core backend features of the Airbnb Clone project.

---

## 1. User Authentication

### ✅ Functional Requirements
- Users can register as `guest` or `host`.
- Users can log in using email/password.
- OAuth (Google, Facebook) support.
- JWT token-based authentication.

### 🔧 API Endpoints

| Method | Endpoint       | Description              |
|--------|----------------|--------------------------|
| POST   | `/api/register` | Register new user        |
| POST   | `/api/login`    | Login and get JWT token  |
| GET    | `/api/profile`  | Get user profile         |

### 📥 Input / Output

**POST /api/register**
```json
// Input
{
  "name": "Rafia",
  "email": "rafia@mail.com",
  "password": "password123",
  "role": "host"
}
