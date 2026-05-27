The uploaded document is an instructional guide about how to analyze and write **Functional Requirements** and **Non-Functional Requirements** for a software system. It explains the concepts, categories, expectations, and—most importantly—what *you are expected to produce*.

Here’s a deep breakdown of what needs to be done.

---

# What the Assignment Actually Wants

You are expected to:

1. **Choose or imagine a software system**

   * Example: online store, food delivery app, hospital system, learning platform, banking app, social media app, etc.
2. **Extract and write Functional Requirements**

   * What the system should DO.
3. **Extract and write Non-Functional Requirements**

   * HOW WELL the system should work.
4. For **each requirement**, write:

   * a **User Requirement**
   * then expand it into a more detailed **System Requirement**

The document repeatedly emphasizes this structure as “very important.”

---

# Part 1 — Functional Requirements

## What are Functional Requirements?

These define:

* services
* features
* operations
* capabilities

that the software must provide.

In simple terms:

> “What should the software do?”

Examples:

* user login
* search
* payment
* notifications
* report generation
* feedback submission

---

# Functional Requirement Categories You Must Cover

The PDF divides functional requirements into categories. Your assignment likely expects you to organize them similarly.

---

## 1. Authentication Requirements

These identify users before they use the system.

You should define things like:

* signup
* login
* password reset
* OTP verification
* biometric login
* Google/Facebook login

### Example

### User Requirement

> The user should be able to log into the system securely.

### System Requirement

> The system shall authenticate users using email and password and optionally support two-factor authentication via OTP.

---

## 2. Authorization / Access Control

Defines what different users can access.

Examples:

* admin permissions
* customer permissions
* teacher/student roles
* read/write/delete access

### Example

### User Requirement

> Admin users should manage all accounts.

### System Requirement

> The system shall provide role-based access control where administrators can create, update, suspend, and delete user accounts.

---

## 3. Data Processing Requirements

These involve:

* input
* validation
* storage
* retrieval
* editing
* deletion

### Example

### User Requirement

> Users should save their profile information.

### System Requirement

> The system shall validate user profile inputs and store them in the database with automatic update support.

---

## 4. User Interface / User Experience Requirements

These describe user interaction and interface behavior.

Examples:

* responsive design
* easy navigation
* menus/buttons
* accessibility
* dashboard layout

### Example

### User Requirement

> Users should navigate the application easily.

### System Requirement

> The system shall provide a responsive dashboard with clearly labeled navigation menus and mobile compatibility.

---

## 5. Reporting Requirements

Generating reports and analytics.

Examples:

* sales reports
* attendance reports
* user activity reports
* export to PDF/Excel

### Example

### User Requirement

> Managers should generate monthly reports.

### System Requirement

> The system shall generate monthly performance reports in PDF and Excel formats.

---

## 6. Third-Party Integration Requirements

Integration with external systems/services.

Examples:

* payment gateway
* cloud storage
* email service
* SMS API
* Google Maps

### Example

### User Requirement

> Users should pay online securely.

### System Requirement

> The system shall integrate with Stripe and PayPal payment gateways for secure online transactions.

---

## 7. Error Handling and Logging

How the system handles failures/errors.

Examples:

* error messages
* logging
* crash handling
* retry mechanisms

### Example

### User Requirement

> Users should receive clear error messages.

### System Requirement

> The system shall log all transaction failures and display descriptive error notifications to users.

---

## 8. Backup and Restore Requirements

Data backup and recovery.

Examples:

* automatic backups
* restore points
* cloud backup
* disaster recovery

### Example

### User Requirement

> User data should not be lost.

### System Requirement

> The system shall perform automated daily backups and support full restoration within 30 minutes.

---

# Important Functional Requirement Rule

The document stresses this:

## First:

Write **User Requirements**

Then:
Expand them into **System Requirements** with implementation details.

This is probably the MOST important grading criterion.

---

# Part 2 — Non-Functional Requirements

## What are Non-Functional Requirements?

These describe:

* quality
* constraints
* performance
* reliability
* behavior

of the system.

In simple terms:

> “How should the software behave?”

Functional = WHAT
Non-functional = HOW WELL

---

# Non-Functional Categories You Must Cover

---

## 1. Usability

Ease of learning and using the system.

Examples:

* simple UI
* understandable menus
* minimal learning curve

### Example

### User Requirement

> The application should be easy to use.

### System Requirement

> New users shall complete registration within 2 minutes without external assistance.

---

## 2. Security

Protection of data and access control.

Examples:

* encryption
* permissions
* secure payment
* privacy protection

### Example

### User Requirement

> User information should remain private.

### System Requirement

> The system shall encrypt all passwords using bcrypt hashing.

---

## 3. Reliability

System stability and fault tolerance.

Examples:

* low failure rate
* uptime
* recovery
* fault detection

### Example

### User Requirement

> The system should work consistently.

### System Requirement

> The system shall maintain 99.9% uptime excluding scheduled maintenance.

---

## 4. Performance

Speed and efficiency.

Examples:

* page load time
* response time
* request handling

### Example

### User Requirement

> Pages should load quickly.

### System Requirement

> The system shall load dashboard pages within 3 seconds under normal load.

---

## 5. Scalability

Ability to handle growth.

### Example

### User Requirement

> The system should support many users.

### System Requirement

> The system shall support 50,000 concurrent users without service degradation.

---

## 6. Availability

Continuous accessibility.

### Example

### User Requirement

> The system should always be accessible.

### System Requirement

> The system shall remain operational 24/7 with scheduled downtime limited to 2 hours monthly.

---

## 7. Compatibility

Works consistently across platforms.

### Example

### User Requirement

> The application should work on all supported devices.

### System Requirement

> The system shall provide identical functionality on Windows 10, Windows 11, Android, and iOS.

---

# What Your Final Submission Should Look Like

A strong submission should have this structure:

---

# 1. Introduction

* Describe the software system briefly.

Example:

> “This project is an online food delivery application.”

---

# 2. Functional Requirements

Organize by categories.

For EACH requirement:

* User Requirement
* System Requirement

Example format:

| ID   | User Requirement               | System Requirement                                                 |
| ---- | ------------------------------ | ------------------------------------------------------------------ |
| FR-1 | Users should register accounts | The system shall support registration using email and phone number |

---

# 3. Non-Functional Requirements

Same structure.

| ID    | User Requirement       | System Requirement                               |
| ----- | ---------------------- | ------------------------------------------------ |
| NFR-1 | Pages should load fast | The system shall load all pages within 3 seconds |

---

# What Teachers Usually Expect

Your work should:

* be organized
* include many realistic requirements
* separate functional/non-functional correctly
* use clear “shall” statements
* contain implementation detail in system requirements
* avoid vague wording

---

# Common Mistakes to Avoid

## ❌ Mixing functional and non-functional

Example:

> “The system should load fast”

This is NON-functional (performance), not functional.

---

## ❌ Writing only features

You must include:

* user requirement
* system requirement

not only feature names.

---

## ❌ Vague requirements

Bad:

> “System should be good.”

Good:

> “The system shall respond within 2 seconds.”

---

# What You Probably Need To Deliver

Most likely:

* 10–20 Functional Requirements
* 5–10 Non-Functional Requirements
* each with:

  * user requirement
  * detailed system requirement

organized in categories.

---

# The Core Idea of the Entire PDF

The entire document teaches this workflow:

1. Understand user needs
2. Convert them into functional requirements
3. Define quality constraints using non-functional requirements
4. Expand user requirements into detailed system requirements

That is the main task you are expected to perform.
