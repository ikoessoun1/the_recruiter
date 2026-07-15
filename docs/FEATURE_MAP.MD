# Feature Map

## Status Legend

* `[ ]` Planned
* `[~]` In Progress
* `[x]` Completed
* `[-]` Deferred

---

# 1. Users Module

## 1.1 Authentication

* [ ] User login
* [ ] Access-token generation
* [ ] Refresh-token generation
* [ ] Access-token refresh
* [ ] User logout
* [ ] Token invalidation
* [ ] Retrieve authenticated user

## 1.2 Password Management

* [ ] Change password
* [ ] Request password reset
* [ ] Verify password-reset identity
* [ ] Reset forgotten password
* [ ] Enforce password rules

## 1.3 Security Questions

* [ ] Set security questions during first login
* [ ] Update security questions
* [ ] Verify security-question answers
* [ ] Use security questions during password reset

## 1.4 Applicant Account Management

* [ ] Register applicant
* [ ] View applicant list
* [ ] View one applicant
* [ ] Update applicant account
* [ ] Search applicants
* [ ] Filter applicants
* [ ] Disable applicant account
* [ ] Soft-delete applicant account
* [ ] Restore applicant account

## 1.5 Administrator Management

* [ ] Create administrator
* [ ] View administrator list
* [ ] View one administrator
* [ ] Update administrator
* [ ] Disable administrator
* [ ] Soft-delete administrator
* [ ] Restore administrator

## 1.6 Roles and Permissions

* [ ] Applicant permissions
* [ ] Administrator permissions
* [ ] Super-administrator permissions
* [ ] Endpoint-level authorization
* [ ] Object-level authorization

---

# 2. Applications Module

## 2.1 Application Creation

* [ ] Create an application for an applicant
* [ ] Prevent duplicate active applications
* [ ] Assign application sections
* [ ] Set initial application status
* [ ] Record application creation date

## 2.2 Application Access

* [ ] Applicant views own application
* [ ] Administrator views one application
* [ ] Administrator lists all applications
* [ ] Search applications
* [ ] Filter applications
* [ ] Paginate application results

## 2.3 Application Editing

* [ ] Update application information
* [ ] Save incomplete application
* [ ] Validate application fields
* [ ] Prevent editing locked applications
* [ ] Prevent unauthorized editing

## 2.4 Application Sections

* [ ] View assigned application sections
* [ ] Save individual sections
* [ ] Update individual sections
* [ ] Track section completion
* [ ] Track section status
* [ ] Submit individual sections
* [ ] Lock individual sections
* [ ] Reopen individual sections

## 2.5 Application Submission

* [ ] Submit complete application
* [ ] Validate required sections
* [ ] Validate required documents
* [ ] Record submission date
* [ ] Prevent duplicate submission
* [ ] Allow correction and resubmission
* [ ] Lock application after final approval

## 2.6 Application Withdrawal

* [ ] Withdraw incomplete application
* [ ] Require withdrawal confirmation
* [ ] Record withdrawal reason
* [ ] Soft-delete withdrawn application
* [ ] Restore application where permitted

## 2.7 Application Status

Possible statuses:

```text
Draft
In Progress
Submitted
Under Review
Changes Requested
Approved
Rejected
Withdrawn
Locked
```

Features:

* [ ] Change application status
* [ ] Validate allowed status transitions
* [ ] Record status-change history
* [ ] Display current application status
* [ ] Display required next action

---

# 3. Application Section Features

## 3.1 Personal Profile

* [ ] Save personal details
* [ ] Update personal details
* [ ] Validate identity details
* [ ] Validate contact information
* [ ] Attach required personal documents

## 3.2 Bank Details

* [ ] Save bank details
* [ ] Update bank details
* [ ] Validate bank account information
* [ ] Restrict access to sensitive bank information

## 3.3 Dependants

* [ ] Add dependant
* [ ] View dependants
* [ ] Update dependant
* [ ] Remove dependant
* [ ] Validate dependant information

## 3.4 Parents

* [ ] Add father information
* [ ] Add mother information
* [ ] Update parent information
* [ ] Prevent duplicate parent types

## 3.5 Emergency Contacts

* [ ] Add emergency contact
* [ ] View emergency contacts
* [ ] Update emergency contact
* [ ] Remove emergency contact
* [ ] Mark primary emergency contact

## 3.6 Academic Qualifications

* [ ] Add academic qualification
* [ ] View qualifications
* [ ] Update qualification
* [ ] Remove qualification
* [ ] Attach academic certificate
* [ ] Validate qualification dates

## 3.7 National Service

* [ ] Add national-service record
* [ ] View national-service record
* [ ] Update national-service record
* [ ] Attach national-service certificate
* [ ] Validate service dates

---

# 4. Reviews Module

## 4.1 Application Review

* [ ] Assign application for review
* [ ] Begin application review
* [ ] View submitted application
* [ ] View individual submitted sections
* [ ] Record reviewer information
* [ ] Record review date

## 4.2 Section Review

* [ ] Approve section
* [ ] Reject section
* [ ] Request section changes
* [ ] Add review comment
* [ ] Lock approved section
* [ ] Reopen section
* [ ] Record section-review history

## 4.3 Complete Application Review

* [ ] Approve complete application
* [ ] Reject complete application
* [ ] Request application changes
* [ ] Add final review message
* [ ] Lock application after approval
* [ ] Record final decision

## 4.4 Review Status

Possible statuses:

```text
Pending
Under Review
Changes Requested
Approved
Rejected
```

Features:

* [ ] Validate review-status transitions
* [ ] Display current review status
* [ ] Filter applications by review status
* [ ] Track unresolved review comments

---

# 5. Documents Module

## 5.1 Document Definitions

* [ ] Define document types
* [ ] Define required documents
* [ ] Associate required documents with sections
* [ ] Mark documents as optional or required
* [ ] Configure accepted file types
* [ ] Configure maximum file size

## 5.2 Document Upload

* [ ] Upload application-level document
* [ ] Upload section-level document
* [ ] Upload record-level document
* [ ] Validate document type
* [ ] Validate file format
* [ ] Validate file size
* [ ] Prevent unauthorized upload

## 5.3 Document Management

* [ ] View uploaded documents
* [ ] Download document
* [ ] Replace document
* [ ] Remove document
* [ ] Soft-delete document
* [ ] Restore document
* [ ] Record document ownership

## 5.4 Downloadable Documents

* [ ] Upload document template
* [ ] List available templates
* [ ] Download document template
* [ ] Restrict template management to administrators

## 5.5 Document Review

* [ ] Approve document
* [ ] Reject document
* [ ] Request replacement
* [ ] Add rejection reason
* [ ] Record reviewer
* [ ] Record review date

---

# 6. Audit Module

## 6.1 User Activity Auditing

* [ ] Record user login
* [ ] Record user logout
* [ ] Record failed authentication attempts
* [ ] Record password changes
* [ ] Record password resets

## 6.2 Application Auditing

* [ ] Record application creation
* [ ] Record application updates
* [ ] Record section submissions
* [ ] Record application submission
* [ ] Record application withdrawal
* [ ] Record application status changes

## 6.3 Review Auditing

* [ ] Record section-review decisions
* [ ] Record application-review decisions
* [ ] Record review comments
* [ ] Record locking and reopening actions

## 6.4 Document Auditing

* [ ] Record document upload
* [ ] Record document replacement
* [ ] Record document deletion
* [ ] Record document review

## 6.5 Audit Access

* [ ] View audit history
* [ ] Filter audit records
* [ ] Search audit records
* [ ] Restrict audit access
* [ ] Prevent audit-record modification
* [ ] Prevent audit-record deletion

---

# 7. Applicant Interface Features

* [ ] Login page
* [ ] First-login security-question page
* [ ] Password-reset page
* [ ] Applicant dashboard
* [ ] Application progress display
* [ ] Application section navigation
* [ ] Section forms
* [ ] Document-upload interface
* [ ] Review-comment display
* [ ] Application-status display
* [ ] Logout action

---

# 8. Administrator Interface Features

* [ ] Administrator login
* [ ] Administrator dashboard
* [ ] Register applicant form
* [ ] Applicant list
* [ ] Applicant details page
* [ ] Application list
* [ ] Application filters
* [ ] Application details page
* [ ] Section-review interface
* [ ] Document-review interface
* [ ] Review-comment form
* [ ] Lock and reopen controls

---

# 9. Super-Administrator Interface Features

* [ ] Administrator list
* [ ] Create administrator form
* [ ] Update administrator form
* [ ] Disable administrator control
* [ ] Restore administrator control
* [ ] Audit-log interface
* [ ] System permission controls

---

# 10. Current Delivery Scope

The complete feature map describes the intended system. Development should only focus on a small active set of features at one time.

## Active Feature

```text
Feature:
Module:
Status:
Goal:
```

## Current Vertical Slice

* [ ] Model
* [ ] Migration
* [ ] Repository
* [ ] Validator
* [ ] Service
* [ ] Serializer
* [ ] API view
* [ ] URL
* [ ] Permissions
* [ ] Unit tests
* [ ] Integration tests
* [ ] API documentation
* [ ] Frontend interface
* [ ] Manual verification

---

# 11. Deferred Features

The following features are outside Version 1:

* [-] Payroll
* [-] Attendance
* [-] Employee performance management
* [-] Public job vacancies
* [-] Candidate sourcing
* [-] Video interviews
* [-] Mobile application
* [-] Advanced analytics
* [-] Multi-organization configuration
