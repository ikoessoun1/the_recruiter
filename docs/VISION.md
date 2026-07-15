```markdown
# Project Vision

## Project Name

**The Recruiter — Mon-Tran Application**

---

## Purpose

The Recruiter is a digital recruitment and applicant onboarding platform designed to reproduce and improve Mon-Tran's existing hiring process.

The system replaces paperwork-heavy workflows with a secure and auditable online process for applicant registration, information collection, document submission, application review, approval management, and applicant communication.

Although the first implementation is designed specifically for Mon-Tran, the system is structured so that other recruitment and human-resource agencies can extend or configure it for similar workflows in the future.

---

## Target Users

The system serves three primary user groups:

- Applicants
- Administrators / Reviewers
- Super Administrators

---

## Problem Statement

Mon-Tran's hiring process involves significant paperwork, repeated communication, manual document handling, and difficulty tracking the current state of an applicant's submission.

The system should reduce these problems by:

- Centralizing applicant and application information.
- Providing secure document submission.
- Supporting structured application review.
- Communicating application status and required next steps.
- Preventing unauthorized changes after submission.
- Maintaining accurate and auditable records.

---

# Core Goals

## Authentication & Account Management

The system must allow authorized users to:

- Sign in securely.
- Refresh authentication sessions.
- Sign out.
- Change their passwords.
- Reset forgotten passwords.
- Configure security questions during first-time account setup.

---

## Applicant Management

Authorized administrators must be able to:

- Register applicants.
- View applicant accounts.
- Search applicants.
- View an individual applicant.
- Update permitted applicant information.
- Disable or soft-delete applicant accounts.

---

## Applicant Application Process

Applicants must be able to:

- Access their assigned application.
- Complete required application sections.
- Save unfinished work.
- Update information while the application remains editable.
- Upload required documents.
- View the current application status.
- Receive review comments and instructions.
- Withdraw or soft-delete an incomplete application where permitted.

---

## Application Administration

Authorized administrators must be able to:

- List applications.
- Search applications.
- Filter applications.
- View complete applications.
- Review submitted sections.
- Approve or reject submissions.
- Add review comments.
- Request corrections.
- Lock applications or individual sections.
- Reopen submissions where authorized.

---

## Super Administration

Super Administrators must be able to:

- Manage applicant accounts.
- Create administrator accounts.
- Update administrator accounts.
- Disable administrator accounts.
- Soft-delete administrator accounts.
- Perform all administrator capabilities.
- Manage high-level system permissions.

---

## Security & Auditability

The system must:

- Restrict actions according to user permissions.
- Protect applicant information and uploaded documents.
- Preserve historical records.
- Record important administrative actions.
- Record review activities.
- Record who performed each action.
- Record when each action occurred.
- Use soft deletion where appropriate.

---

# Project Principles

- Functionality is more important than visual complexity.
- The interface should remain simple and usable.
- Business rules belong primarily in the backend.
- Important actions should always be auditable.
- Modules should have clearly defined responsibilities.
- Features should be developed as complete vertical slices.
- Maintainability is preferred over unnecessary abstraction.

---

# Non-Goals (Version 1)

The first version of the project will **not** include:

- Payroll processing.
- Attendance management.
- Employee performance management.
- Public job-board functionality.
- Candidate sourcing.
- Video interviewing.
- Accounting.
- Advanced analytics.
- Mobile applications.
- Extensive UI customization.

---

# Technology Stack

## Backend

- Python
- Django
- Django REST Framework
- PostgreSQL

## Frontend

- React
- TypeScript

## Supporting Tools

- Git
- GitHub
- REST APIs
- JWT Authentication
- Backend Testing

---

# Version 1 Scope

The first release focuses solely on reproducing Mon-Tran's recruitment workflow.

The goal is to build a stable, maintainable system that accurately models the organization's existing hiring process before introducing configurable workflows or multi-organization support.
```
