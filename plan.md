The list of systems you can choose for your Systems Analysis and Design course project, along with some of the main features of each system, is as follows:

1. **Online Library Management System**
   Book search, borrowing and returning books, member management, book reservation, and late fee registration.
2. **Health and Fitness Application**
   Recording workout activities, training programs, calorie and health monitoring, diet management, and progress reports.
3. **Event Management System (conferences, workshops, concerts, etc.)**
   Participant registration, ticket sales, event scheduling, hall management, and notification sending.
4. **Smart Home Device Automation and Management System**
   Control of smart devices, scheduling device operations, monitoring energy consumption, and home security management.
5. **Warehouse and Inventory Management System for Large Companies**
   Recording incoming and outgoing goods, inventory management, reporting, product tracking, and supply order management.
6. **Social Media Data Analytics Software**
   User sentiment analysis, trend detection, user activity analysis, influencer identification, and data visualization.
7. **Task and Project Management System**
   Defining and assigning tasks, determining user roles, tracking project progress, managing delays, and team performance reporting.
8. **Hospital Management and Medical Appointment System**
   Patient information registration, appointment booking and management, medical record registration, patient referral to doctors, and insurance/payment management.
9. **Learning Management System (LMS) for Universities and Schools**
   Conducting virtual classes, course management, assignment submission and retrieval, online exams, and grade recording.
10. **Online Banking System** (Chosen Case Study)
    Managing bank accounts, money transfers, transaction viewing, bill payments, and secure user authentication.
11. **Transportation Ticket Reservation and Sales System**
    Route searching, ticket booking and purchasing, vehicle capacity management, online payment, and travel status tracking.

Please carefully choose one of these systems for your project.

The items requested from you in the first phase of the project are:

1. Extracting and analyzing the requirements of the selected software system.
2. Identifying the functional requirements of the selected software system and presenting them in the form of user requirements.
3. Adding implementation details and technical information to the functional requirements and presenting them in the form of system requirements.
4. Identifying the non-functional requirements of the selected software system and presenting them in the form of user requirements.
5. Adding implementation details and technical information to the non-functional requirements and presenting them in the form of system requirements.

Also:

Please submit the first phase of the project (extracting functional and non-functional requirements in the form of user requirements and system requirements) no later than 24:00 on Friday of next week, Khordad 8, 1405.

After extracting the requirements, please send the files according to the following instructions:

1. Place the Word or PDF file inside a folder and compress it into a ZIP file.
2. Along with the submitted file, your description must be written in English in the following format, and after uploading the file, it should be included as the descriptive text beside the file:

`First name, last name, ID, SAD, project name, phase 1`

For example:

`Morteza Jaderyan, 40298256, SAD, Hospital, phase 1`

Also, dear students,

All project deliverables must be submitted in electronic format (Word or PDF files). Otherwise, no grade will be assigned.

In addition, in the recorded video file that was sent to you yesterday, it was fully explained that you must choose a specific format and structure for presenting the requirements.

Therefore, selecting an appropriate format and structure for organizing the functional and non-functional requirements—so that the distinction between these two categories is clearly demonstrated in the best possible way—will be considered part of your project grade.

---

# 📚 Expanded Specification Blueprint & Grading Rubric (Derived from req.md)

To achieve the highest marks on this assignment, the following structuring rules, taxonomy, and content expectations must be met.

## 🎯 Target Volumes
*   **Functional Requirements (FRs):** 10 – 20 distinct requirements.
*   **Non-Functional Requirements (NFRs):** 5 – 10 distinct requirements.

---

## 🗂️ Required Requirements Categorization

### 1. Functional Requirement Categories (What the System Shall Do)
Your requirements must be grouped under these **8 core operational categories**:
1.  **Authentication:** Signup, Login, MFA, biometric checks, secure token generation.
2.  **Authorization & Access Control:** Role-Based Access Control (RBAC), specific admin, operator, and customer privileges.
3.  **Data Processing:** Inputs, validations, secure storage, CRUD operations, database queries.
4.  **UI/UX:** Responsive layout, clean dashboards, navigation speed, visual accessibility.
5.  **Reporting:** Automated statements, sales/ledger reports, exports (PDF/CSV).
6.  **Third-Party Integrations:** Payment gateway APIs, SMS alert microservices, authentication servers.
7.  **Error Handling & Logging:** Client-side input validation, error notification banners, system server exception logging.
8.  **Backup & Restore:** Automated daily system snapshots, disaster recovery protocols.

### 2. Non-Functional Requirement Categories (How Well the System Behaves)
Your quality constraints must be organized into these **7 core system behaviors**:
1.  **Usability:** Intuitiveness, learning curve limit (e.g., onboarding times), accessibility compliance.
2.  **Security:** Encryption standards (bcrypt, TLS 1.3, AES-256), session timeouts.
3.  **Reliability:** Fault tolerance, database recovery speed, low failure rates.
4.  **Performance:** Page load speeds, transaction response times, latency limits.
5.  **Scalability:** Maximum concurrent users, load handling without system degradation.
6.  **Availability:** Service uptime SLAs (e.g., 99.9% availability, scheduled downtime windows).
7.  **Compatibility:** Full multi-platform consistency (Web, Android, iOS, Windows).

---

## 📝 Document Formatting & Structural Layout

The final PDF/Word deliverable must be formatted strictly around these three core sections:

### Section 1: Introduction
*   A concise, high-level summary of the system, its main scope, user base, and utility.

### Section 2: Functional Requirements
Organize each functional requirement into a structured comparison table using clear, implementable **System-level "shall" statements**:

| ID | Category | User Requirement | System Requirement (Technical details & "Shall" wording) |
| :--- | :--- | :--- | :--- |
| **OBS-FR-01** | Authentication | The user should be able to log in securely. | The system shall authenticate users using their registered email and encrypted password, forcing multi-factor authentication (MFA) via a 6-digit SMS OTP. |
| **OBS-FR-02** | Reporting | Customers should be able to download their history. | The system shall compile a customer's transaction history into a standard PDF file format and download it within 5 seconds of the user request. |

### Section 3: Non-Functional Requirements
Follow the same structured format for quality attributes:

| ID | Category | User Requirement | System Requirement (Quantitative & Testable details) |
| :--- | :--- | :--- | :--- |
| **OBS-NFR-01** | Performance | The bank app should load fast. | The system shall load the customer dashboard pages within 3 seconds under normal network conditions. |
| **OBS-NFR-02** | Security | My account information should be safe. | The system shall encrypt all sensitive customer data at rest using the AES-256 standard and hashing all credentials with bcrypt. |

---

## ⚠️ Critical Pitfalls & Checklist for Grading
*   [ ] **No Mixing:** Ensure all Performance, Security, and Availability rules are in the NFR section, not FR.
*   [ ] **Explicit Dual-Layer Structure:** Do not write just a single requirement sentence. Every single requirement **must** have both a *User Requirement* and an expanded *System Requirement*.
*   [ ] **Quantitative NFRs:** Avoid vague words like "good", "fast", or "secure". Specify precise metrics (e.g., "within 2 seconds", "99.99% uptime", "TLS 1.3").
*   [ ] **Strict "Shall" Verbiage:** Ensure system requirements use the engineering keyword "**shall**" to represent absolute system obligations.
