# 2. Personal Data 👤

## What is personal data?

Personal data is information relating to an identified or identifiable natural person.

In simple words:

> **If information can identify or relate to a person, it may be personal data.**

---

# Examples of Personal Data

### Direct identifiers

These can identify someone directly.

```text
Name
Email address
Phone number
Passport number
Customer ID
```

### Other information

Some information may identify or relate to someone when combined with other information.

```text
IP address
Location data
Cookie identifiers
Device identifiers
Online identifiers
```

The exact classification depends on context.

---

# Example

Suppose we have:

```text
Name: Rahul
Age: 22
City: Ahmedabad
```

The name obviously relates to Rahul.

But even something like:

```text
Customer ID: C102938
```

can be personal data if the organization can connect that ID to Rahul.

---

# What is NOT necessarily personal data?

Information that cannot reasonably be linked to an identifiable person may not be personal data.

Example:

```text
Company's total number of customers = 50,000
```

If the number is genuinely anonymous and cannot be used to identify individuals, it may not be personal data.

---

# Personal Data vs Sensitive Data

GDPR has a category called **special categories of personal data** that receives additional protection.

Examples include:

```text
Racial or ethnic origin
Political opinions
Religious or philosophical beliefs
Trade union membership
Genetic data
Certain biometric data
Health data
Sex life
Sexual orientation
```

Processing these categories generally requires a specific GDPR exception in addition to a lawful basis.

---

# Simple Example

Suppose MyShop asks:

```text
Name
Email
Address
```

These are normal examples of personal data.

Now imagine MyShop asks:

```text
Health condition
Religious beliefs
Biometric identifier
```

These can involve special-category data and require much more careful handling.

---

# Easy Test

Whenever you see a piece of information, ask:

> **"Can this information identify or relate to a person?"**

If yes:

```text
Think → PERSONAL DATA
```

---

# Personal Data Example for Developers

Consider this Java class:

```java
class User {

    int id;
    String name;
    String email;
    String phone;
    String address;
}
```

Several of these fields contain personal data.

Therefore, a developer should think about:

```text
Collection
Storage
Access
Security
Retention
Deletion
User rights
```

---

# Important Lesson

Don't think:

> "It's just a database field."

Instead think:

> "This database field may contain someone's personal data."

That mindset is important for privacy-aware development.
