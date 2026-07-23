# Authentication Flow

## Login Flow

User

↓

Enter Email & Password

↓

Spring Security Authentication Filter

↓

Authentication Manager

↓

UserDetailsService

↓

Database Validation

↓

BCrypt Password Verification

↓

JWT Token Generated

↓

Token Returned to Client

↓

Client Stores JWT

↓

Every Request

↓

Authorization Header

↓

JWT Filter

↓

Spring Security Context

↓

Protected API

---

## Registration Flow

User

↓

Registration Form

↓

Validation

↓

Password Encryption (BCrypt)

↓

Save User

↓

Return Success Response