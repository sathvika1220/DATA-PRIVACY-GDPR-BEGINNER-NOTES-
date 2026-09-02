# 7. Data Breaches 🚨

## What is a data breach?

A personal data breach is a security incident involving personal data.

It can involve:

```text
Unauthorized access
Unauthorized disclosure
Loss
Destruction
Alteration
```

A breach can be accidental or unlawful.

---

# Example 1 — Hacker Attack

```text
Company database
      ↓
Hacker gains unauthorized access
      ↓
Customer information exposed
```

This may be a personal data breach.

---

# Example 2 — Wrong Email

An employee accidentally sends:

```text
Customer list
```

to the wrong person.

Even though there was no hacker, personal data was disclosed to an unauthorized recipient.

This can still be a personal data breach.

---

# Example 3 — Lost Laptop

An employee loses a laptop containing personal data.

Depending on the circumstances, this can constitute a personal data breach.

---

# What should an organization do?

A company should have a process for:

```text
Detect
  ↓
Investigate
  ↓
Contain
  ↓
Assess risk
  ↓
Document
  ↓
Notify when required
  ↓
Fix the problem
```

---

# The 72-Hour Rule

This is an important GDPR concept.

Where a personal data breach is likely to result in a risk to individuals' rights and freedoms, the controller generally must notify the competent supervisory authority:

> **Without undue delay and, where feasible, within 72 hours after becoming aware of it.**

If notification is late, reasons for the delay should be provided.

Not every breach automatically requires notification to the authority.

---

# What about the affected people?

If the breach is likely to result in a **high risk** to individuals' rights and freedoms, the affected individuals may also need to be informed, subject to GDPR exceptions.

---

# Example

Suppose a hospital database is hacked.

Data exposed:

```text
Patient names
Medical information
Contact details
```

This could create significant risks.

The organization needs to:

```text
Investigate
↓
Contain the incident
↓
Assess the risk
↓
Notify the authority if required
↓
Notify affected people if the high-risk conditions apply
↓
Take corrective measures
```

---

# Controller vs Processor During a Breach

Suppose:

```text
MyShop
   ↓
Uses Cloud Provider
```

Cloud provider discovers a breach.

The processor generally needs to notify the controller without undue delay.

The controller then assesses its own notification obligations.

---

# Important Developer Lesson

Security isn't something you think about only after a breach.

Build security into the application:

```text
Authentication
Authorization
Encryption
Secure passwords
Access controls
Logging
Monitoring
Backups
Security testing
```

---

# Easy Memory

Remember:

> **DETECT → ASSESS → CONTAIN → NOTIFY → FIX**

And remember:

> **72 hours applies to certain reportable breaches, not every breach.**
