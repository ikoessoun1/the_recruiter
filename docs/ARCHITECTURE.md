````markdown
# System Architecture

## Overview

The Recruiter is organized as a modular monolith.

Each business domain is implemented as an independent Django application (module) with clearly defined responsibilities. Modules communicate through service interfaces rather than directly manipulating another module's internal implementation whenever possible.

---

# Architectural Principles

- Every module owns its own business logic.
- Modules should have a single responsibility.
- Business rules belong in services.
- Database access belongs in repositories.
- Views should remain thin.
- Validation should occur before persistence.
- APIs communicate through serializers.
- Modules should avoid circular dependencies.

---

# Module Overview

## Accounts

**Responsibility**

Authentication, authorization, and user management.

### Owns

- User accounts
- Roles
- Permissions
- Authentication
- Password management
- Security questions

### Provides

- Login
- Logout
- Refresh token
- Password reset
- User permissions

---

## Applications

**Responsibility**

Manages applicant applications and all application sections.

### Owns

- Applications
- Sections
- Application lifecycle
- Submission state

### Depends On

- Users
- Documents
- Reviews

---

## Reviews

**Responsibility**

Handles administrator review of submitted applications.

### Owns

- Review decisions
- Review comments
- Approval workflow
- Locking submissions

### Depends On

- Applications

---

## Documents

**Responsibility**

Manages uploaded and generated documents.

### Owns

- Uploaded files
- Document definitions
- Downloadable templates
- Document validation

### Depends On

- Applications
- Users

---

## Audit

**Responsibility**

Records important system actions.

### Owns

- Audit logs
- Change history
- Administrative actions

### Depends On

- All modules

---

# Module Dependencies

```text
Users
│
├── Applications
│      │
│      ├── Reviews
│      │
│      └── Documents
│
└── Audit
```

Audit may observe every module.

Other modules should not depend on Audit.

---

# Request Flow

Every API request follows the same flow.

```text
Client

↓

View

↓

Serializer

↓

Service

↓

Repository

↓

Database
```

### Responsibilities

**View**

- Receive request
- Call serializer
- Return response

**Serializer**

- Convert request/response data

**Service**

- Business logic
- Validation coordination
- Transaction management

**Repository**

- Database operations only

**Database**

- Persistent storage

---

# Standard Module Structure

```text
module/

├── models/
├── repositories/
├── services/
├── serializers/
├── views/
├── validators/
├── exceptions/
├── tests/

├── urls.py
├── admin.py
├── apps.py
```

---

# Dependency Rules

Allowed

Service → Repository

View → Service

Serializer → Service

Repository → Models

Not Allowed

Repository → View

Repository → Serializer

View → Repository

Models → Services

Modules with circular dependencies

---

# Future Modules

The following modules may be introduced in future versions:

- Employees
- Notifications
- Reporting
- Configuration
- Dashboard
````
