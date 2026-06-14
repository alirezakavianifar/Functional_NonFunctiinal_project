After thoroughly reviewing both your **Phase 1 Requirements Specification** and the **Phase 2 project instructions**, the second phase is essentially focused on **system modeling** rather than requirements engineering. Your Phase 1 is already complete and provides enough information to derive all required models.

## What Phase 2 Requires

According to the project description, you must produce three major deliverables:

### 1. Context Model (Operational Context / Operational Boundary)

You must identify the operational boundary of the Online Banking System and show the major internal and external subsystems interacting with it.

### 2. Use Case Diagrams

You must extract **8 important use cases** from the functional requirements and draw the corresponding Use Case Diagrams.

### 3. Activity Diagrams

You must either:

* Draw an Activity Diagram for each selected Use Case, OR
* Draw Activity Diagrams for the activities performed inside each subsystem shown in the Context Model.

---

# Recommended Context Model

The Online Banking System already defines its operational scope and major modules.

I recommend the following Context Model.

### Central System

**Online Banking System (OBS)**

### Internal Subsystems

1. Authentication & MFA Subsystem
2. Account Management Subsystem
3. Funds Transfer Subsystem
4. Bill Payment Subsystem
5. Reporting & Statement Subsystem
6. Notification Subsystem
7. Audit & Logging Subsystem
8. Backup & Recovery Subsystem

### External Systems

1. Customer
2. Corporate Customer
3. System Administrator
4. Bank Teller
5. Shetab / ACH / RTGS Network
6. SMS Gateway
7. Utility Providers
8. Identity Verification Service

These are directly supported by the Phase 1 specification.

---

# Recommended 8 Use Cases

The project requires only eight important use cases.

I recommend:

| UC  | Use Case                | Main Actor                    |
| --- | ----------------------- | ----------------------------- |
| UC1 | Register Account        | Customer                      |
| UC2 | Login with MFA          | Customer / Corporate Customer |
| UC3 | View Account Balance    | Customer                      |
| UC4 | Transfer Funds          | Customer                      |
| UC5 | Pay Utility Bills       | Customer                      |
| UC6 | Generate Statement      | Customer                      |
| UC7 | Manage Backups          | System Administrator          |
| UC8 | Review Transaction Logs | Bank Teller / Administrator   |

These are derived directly from the major functional requirements and system modules.

---

# IMPORTANT REQUIREMENT FOR YOUR USE CASE DIAGRAMS

🛑 **Actors must be drawn as stick-figure humans (UML Actor notation).**

Do **NOT** use:

* rectangles
* icons
* images
* text labels alone

Use the standard UML actor symbol for:

* Customer
* Corporate Customer
* System Administrator
* Bank Teller

Even if you use tools such as Draw.io, StarUML, Visual Paradigm, Lucidchart, or Enterprise Architect, the actor representation must be the UML stick figure.

For external systems (SMS Gateway, Shetab API, Utility Provider), I recommend also showing them as actors because the Phase 2 instructions explicitly allow external systems to be actors in use-case interactions.

---

# Recommended Use Case Relationships

### Register Account

Include:

* Validate National ID
* Setup MFA
* Send OTP

Use:

* <`<include>`>

---

### Login with MFA

Include:

* Validate Credentials
* Verify OTP
* Generate Session

Use:

* <`<include>`>

---

### Transfer Funds

Include:

* Validate Balance
* Validate Destination Account
* Send SMS Notification

Use:

* <`<include>`>

---

### Pay Utility Bills

Include:

* Verify Utility Bill
* Debit Account
* Generate Receipt

Use:

* <`<include>`>

---

### Generate Statement

Include:

* Filter Transactions
* Generate PDF
* Download Statement

Use:

* <`<include>`>

---

# Activity Diagrams (Recommended)

I strongly recommend choosing the first option from the project instructions and creating Activity Diagrams for each selected Use Case.

That gives you:

### AD1 – Register Account

Start → Enter Information → Validate Data → Send OTP → Verify OTP → Create Account → End

### AD2 – Login with MFA

Start → Enter Credentials → Validate Password → Send OTP → Verify OTP → Create Session → End

### AD3 – View Balance

Start → Request Balance → Retrieve Ledger → Display Balance → End

### AD4 – Transfer Funds

Start → Enter Transfer → Validate Balance → Validate Destination → Execute Transfer → Generate Receipt → End

### AD5 – Pay Utility Bill

Start → Select Utility → Fetch Bill → Validate Funds → Pay Bill → Send Confirmation → End

### AD6 – Generate Statement

Start → Select Date Range → Query Transactions → Generate PDF → Download PDF → End

### AD7 – Manage Backups

Start → Schedule Backup → Encrypt Backup → Store Offsite → Verify Backup → End

### AD8 – Review Transaction Logs

Start → Search Logs → Retrieve Records → Analyze Activity → Export Report → End

---

# Deliverables Checklist

Your final Phase 2 submission should contain:

### Section 1

✅ Context Model Diagram

### Section 2

✅ Combined Use Case Diagram (8 use cases)

or

✅ 8 separate Use Case Diagrams

### Section 3

✅ 8 Activity Diagrams

### Section 4

✅ Short explanation below each diagram (1–2 paragraphs)

### UML Rule

✅ Actors represented with **stick-figure human symbols** only.

This approach will fully satisfy the requirements described in the Phase 2 document while remaining consistent with the Online Banking System specification developed in Phase 1.
