# 3. Data Processing 🔄

## What does "processing" mean?

In GDPR, processing is a very broad concept.

It includes many operations performed on personal data.

For example:

```text
Collecting
Recording
Organizing
Storing
Using
Viewing
Sharing
Changing
Retrieving
Deleting
```

---

# Simple Example

A user creates an account:

```text
User enters email
       ↓
Application collects email
       ↓
Database stores email
       ↓
Application retrieves email
       ↓
Email service sends confirmation
       ↓
Account is eventually deleted
```

There are multiple processing activities here.

---

# Processing does NOT mean only "changing data"

A common beginner mistake is:

> "Processing means modifying data."

Not necessarily.

Simply:

```text
Storing data
```

can be processing.

Similarly:

```text
Viewing data
```

can be processing.

---

# Example: Employee Database

A company stores:

```text
Employee ID
Name
Email
Salary
Address
```

The following can all involve processing:

### Adding employee

```text
INSERT employee
```

### Viewing employee

```text
SELECT employee
```

### Updating employee

```text
UPDATE employee
```

### Sharing information

```text
Send information to authorized payroll provider
```

### Deleting employee data

```text
DELETE employee
```

---

# Processing in a Web Application

Imagine a Spring Boot application:

```text
Frontend
   ↓
REST API
   ↓
Service
   ↓
Repository
   ↓
Database
```

A user's personal data may pass through several components.

For example:

```text
React
 ↓
POST /users
 ↓
UserController
 ↓
UserService
 ↓
UserRepository
 ↓
Database
```

A privacy-aware developer should understand where personal data flows.

---

# Data Flow Example

```text
             USER
              │
              ↓
          Web Form
              │
              ↓
          REST API
              │
              ↓
          Application
              │
       ┌──────┴──────┐
       ↓             ↓
   Database      Email Service
       │
       ↓
   Backup System
```

The important question is:

> **Where is personal data going?**

---

# Why Data Flow Matters

Suppose a user enters:

```text
email@example.com
```

You need to know:

```text
Where is it stored?
Who can access it?
Is it sent to another service?
How long is it retained?
How is it protected?
```

---

# Easy Memory

> **Processing = Doing something with personal data.**

If you're unsure whether something is processing, ask:

> **"Am I doing something with personal data?"**

If yes, it may be processing under GDPR.
