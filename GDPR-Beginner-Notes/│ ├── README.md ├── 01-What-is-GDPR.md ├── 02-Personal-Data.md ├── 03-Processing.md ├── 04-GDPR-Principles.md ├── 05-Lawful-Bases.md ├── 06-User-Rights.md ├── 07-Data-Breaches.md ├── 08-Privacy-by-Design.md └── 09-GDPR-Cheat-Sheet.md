# 1. What is GDPR? 🔐

## What does GDPR mean?

**GDPR** stands for:

> **General Data Protection Regulation**

It is an EU regulation designed to protect individuals when their personal data is processed and to give individuals rights and control over their personal data.

GDPR became applicable on **25 May 2018**.

---

# Why was GDPR introduced?

Before thinking about the law, think about how much information companies collect about people.

For example, an online shopping website may know:

```text
Name
Email
Phone number
Address
Order history
IP address
Payment-related information
```

A social media platform may know:

```text
Name
Photos
Location information
Interests
Messages
Device information
```

This information can be valuable and sensitive.

GDPR establishes rules around how organizations handle personal data.

---

# Simple Example

Imagine we create an online shopping website called:

**MyShop**

When Rahul creates an account, MyShop collects:

```text
Name: Rahul
Email: rahul@example.com
Phone: 9876543210
Address: Ahmedabad
```

GDPR makes us ask:

### Why are we collecting this?

```text
Name → Identify the customer
Email → Account/order communication
Phone → Delivery communication
Address → Deliver the product
```

We shouldn't simply collect information because:

> "Maybe we will need it someday."

---

# GDPR is about the entire data lifecycle

Think about data moving through your application:

```text
COLLECT
   ↓
STORE
   ↓
USE
   ↓
SHARE
   ↓
UPDATE
   ↓
ARCHIVE / DELETE
```

GDPR can apply throughout this lifecycle.

---

# Does GDPR apply only to European companies?

No.

GDPR can apply to organizations outside the EU when their processing falls within its territorial scope, such as certain situations involving offering goods or services to people in the EU or monitoring their behaviour.

For example:

```text
Company
India 🇮🇳
   ↓
Offers services to people in EU 🇪🇺
   ↓
Processes their personal data
```

Depending on the circumstances, GDPR may apply.

---

# Important GDPR Terms

## 1. Data Subject

The person whose personal data is being processed.

Example:

```text
Rahul creates an account
        ↓
Rahul = Data Subject
```

---

## 2. Controller

The organization that determines the purposes and means of processing personal data.

Example:

```text
MyShop decides:

Why do we need the customer's address?
→ Product delivery

Why do we need email?
→ Order communication
```

MyShop is acting as the **Controller**.

---

## 3. Processor

A processor processes personal data on behalf of a controller.

Example:

```text
MyShop
   ↓
Uses a cloud provider
   ↓
Cloud provider processes/stores data
```

Conceptually:

```text
MyShop → Controller
Cloud provider → Processor
Customer → Data Subject
```

The actual legal relationship depends on the specific services and processing arrangements.

---

# Controller vs Processor

| Role         | Simple meaning                         |
| ------------ | -------------------------------------- |
| Data Subject | Person whose data is processed         |
| Controller   | Decides why/how data is processed      |
| Processor    | Processes data on behalf of controller |

### Easy way to remember:

> **Subject = Person**
>
> **Controller = Decides**
>
> **Processor = Does the processing**

---

# GDPR in one sentence

> **GDPR is about responsible handling of people's personal data and protecting their rights.**
