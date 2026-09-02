# 8. Privacy by Design 🏗️🔐

## What is Privacy by Design?

Privacy by Design means:

> **Think about privacy while designing and building the system — not after the system is finished.**

GDPR also includes the concept of **data protection by design and by default**.

---

# Bad Approach

Imagine a developer creates an application:

```text
Build application
       ↓
Collect everything
       ↓
Store everything
       ↓
Launch
       ↓
"Oh! We need privacy."
```

This can create unnecessary risks.

---

# Better Approach

Before building:

```text
What data do we need?
        ↓
Why do we need it?
        ↓
Who needs access?
        ↓
How long should we keep it?
        ↓
How should we protect it?
        ↓
What happens when the user deletes their account?
```

Then design the application.

---

# Example: Registration Form

## Bad design

```text
Registration

Name
Email
Phone
Address
Passport number
Aadhaar number
Blood group
Religion
Favorite movie
```

Why are we collecting all of this?

If the application only needs:

```text
Name
Email
Password
```

then the other fields may be unnecessary.

---

# Better Design

```text
Registration

Name
Email
Password
```

Collect only what is necessary for the intended purpose.

---

# Privacy by Default

Privacy should also be considered in the application's default settings.

### Example

Imagine a social media application.

Bad default:

```text
Profile → Public
Location → Shared
Email → Public
Phone → Public
```

A privacy-conscious design might use more protective defaults and let users intentionally choose broader sharing where appropriate.

---

# Developer Example

Suppose you're building a Spring Boot API.

```text
POST /users
```

Request:

```json
{
    "name": "Rahul",
    "email": "rahul@example.com",
    "phone": "9876543210"
}
```

Ask:

```text
Do we need phone?
Who can access it?
Should it appear in API responses?
Should logs contain it?
How long should it be retained?
```

---

# Don't Put Personal Data in Logs

Bad:

```text
System.out.println(
    "User login: " + email + " password=" + password
);
```

Never log passwords.

Be careful with:

```text
Email
Phone
Tokens
Addresses
Authentication information
```

---

# Access Control

Not every employee should have access to every customer's information.

Example:

```text
Customer Support
     ↓
Needs limited customer information

Finance
     ↓
Needs billing information

Developer
     ↓
Should not automatically have unrestricted production access
```

Use appropriate authorization and least-privilege principles.

---

# Encryption

Where appropriate, use encryption to protect data.

For example:

```text
Application
    ↓
Encrypted connection
    ↓
Database
```

Encryption is not the entire GDPR solution, but it is an important security measure.

---

# Privacy by Design Checklist

Before launching an application, ask:

```text
☐ What personal data do we collect?
☐ Why do we collect it?
☐ Is each field necessary?
☐ Who can access it?
☐ How is it protected?
☐ How long is it retained?
☐ Can users update their data?
☐ Can applicable deletion requests be handled?
☐ Are logs exposing personal data?
☐ Are third-party services involved?
```

---

# Easy Memory

> **Don't build first and think about privacy later.**

Instead:

> **BUILD WITH PRIVACY FROM DAY ONE.**
