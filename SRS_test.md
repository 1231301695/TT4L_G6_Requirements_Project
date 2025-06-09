![](media/image69.png){width="4.791666666666667in" height="1.65625in"}

**CSE 6224 -- Software Requirement Engineering**

_Trimester 2510_

Tutorial Session : TT4L

Group Number: G2

Leader: Iman Nadhirah binti Mohd Hafiz

Submission Date: 25/5/2025

**Group members:**

---

**NO** **STUDENT ID** **NAME**

---

**1** **1211111073** **IMAN NADHIRAH BINTI MOHD HAFIZ**

**2** **1211112294** **PHARTIBAN A/L KUMARHESAN**

**3** **1211112191** **SUZANNAH PANCER**

**4** **1211108832** **NURUL NATASHA ADILYN BINTI FADZIL**

---

Software Requirement\
Specification

![](media/image71.png){width="4.505208880139983in"
height="2.4598436132983377in"}

EduAxis:

University Communication and Services Portal

Version: 1.0

Release Date: 25th May 2025

# Table of Contents

[**Table of Contents 2**](#table-of-contents)

[**1. Introduction 7**](#introduction)

> [1.1 Purpose 7](#purpose)
>
> [1.2 Scope 7](#scope)
>
> [1.3 Product overview 8](#product-overview)
>
> [1.3.1 Product perspective 8](#product-perspective)
>
> [1.3.1.1 System interfaces 9](#system-interfaces)
>
> [1.3.1.2 User interfaces 12](#user-interfaces)
>
> [1.3.1.3 Hardware interfaces 14](#hardware-interfaces)
>
> [1.3.1.4 Software interfaces 15](#software-interfaces)
>
> [1.3.1.5 Communication Interfaces 18](#communication-interfaces)
>
> [1.3.1.6 Memory constraints 20](#memory-constraints)
>
> [1.3.1.7 Operations 22](#operations)
>
> [1.3.1.8 Site adaptation requirements
> 24](#site-adaptation-requirements)
>
> [1.3.1.9 Interfaces with services 26](#interfaces-with-services)
>
> [1.3.2 Product functions 27](#product-functions)
>
> [1.3.2.1 Student function 29](#student-function)
>
> [1.3.2.2 Parent function 52](#parent-function)
>
> [1.3.2.3 Lecturer function 64](#lecturer-function)
>
> [1.3.2.4 Administrator function 79](#administrator-function)
>
> [1.3.3 User Characteristics 91](#user-characteristics)
>
> [1.3.3.1 Student 91](#student)
>
> [1.3.3.2 Parent or Guardian 91](#parent-or-guardian)
>
> [1.3.3.3 Lecturer 91](#lecturer)
>
> [1.3.3.4 Administrator 92](#administrator)
>
> [1.3.4 Limitations 93](#limitations)

[**2. References 94**](#references)

[**3. Requirements 95**](#requirements)

> [3.1 Apportioning of Requirements 95](#apportioning-of-requirements)
>
> [3.1.1 Student Module 95](#student-module)
>
> [3.1.2 Parent Module 95](#parent-module)
>
> [3.1.3 Lecturer Module 96](#lecturer-module)
>
> [3.1.4 Admin Module 96](#admin-module)
>
> [3.2 External interfaces 97](#external-interfaces)
>
> [3.2.1 University Database Interface
> 97](#university-database-interface)
>
> [3.2.2 Campus Management System (CLiC) Interface
> 97](#campus-management-system-clic-interface)
>
> [3.2.3 Learning Management System (LMS) Interface
> 98](#learning-management-system-lms-interface)
>
> [3.2.4 SMS & Email Gateway Interface 98](#sms-email-gateway-interface)
>
> [3.2.5 Authentication Service Interface
> 99](#authentication-service-interface)
>
> [3.2.6 Payment Gateway Interface 99](#payment-gateway-interface)
>
> [3.3 Elicitation Techniques Based on Kano Model
> 100](#elicitation-techniques-based-on-kano-model)
>
> [3.4 Functional Requirements 101](#functional-requirements)
>
> [3.4.1 Dissatisfier Requirements 101](#dissatisfier-requirements)
>
> [3.4.2 Satisfier Requirements 104](#satisfier-requirements)
>
> [3.4.3 Delighter Requirements 106](#delighter-requirements)
>
> [3.5 Performance requirements 107](#performance-requirements)
>
> [3.5.1 Static Numerical Requirements
> 107](#static-numerical-requirements)
>
> [3.5.2 Dynamic Numerical Requirements
> 108](#dynamic-numerical-requirements)
>
> [3.6 Usability Requirements 109](#usability-requirements)
>
> [3.6.1 User Interface 109](#user-interface)
>
> [3.6.2 User Experience 109](#user-experience)
>
> [3.6.3 Communication 109](#communication)
>
> [3.6.4 Data protection 110](#data-protection)
>
> [3.7 Logical Database Requirements
> 111](#logical-database-requirements)
>
> [3.7.1 Class Diagram 111](#class-diagram)
>
> [3.7.2 Data Entities 112](#_xh9314f7iyxn)
>
> [3.7.3 Relationship 114](#relationship)
>
> [3.7.4 Types of Information Used by Various Functions
> 115](#types-of-information-used-by-various-functions)
>
> [3.7.5 Frequency of Use 116](#frequency-of-use)
>
> [3.7.6 Accessing Capabilities 117](#accessing-capabilities)
>
> [3.7.7 Integrity Constraints 118](#integrity-constraints)
>
> [3.7.8 Security 118](#security)
>
> [3.7.9 Data Retention Requirements 119](#data-retention-requirements)
>
> [3.9 Design Constraints 120](#design-constraints)
>
> [3.9.1 Compliance with Data Privacy Regulations
> 120](#compliance-with-data-privacy-regulations)
>
> [3.9.2 Integration with Existing University Systems
> 120](#integration-with-existing-university-systems)
>
> [3.9.3 Security Standards 120](#security-standards)
>
> [3.9.4 Accessibility Requirements 120](#accessibility-requirements)
>
> [3.9.5 API Usage Limitations 121](#api-usage-limitations)
>
> [3.9.6 Performance and Scalability 121](#performance-and-scalability)
>
> [3.9.7 User Experience Consistency 121](#user-experience-consistency)
>
> [3.9.8 Data Interoperability 121](#data-interoperability)
>
> [3.9.9 Legal and Ethical Considerations
> 122](#legal-and-ethical-considerations)
>
> [3.9.10 Project Budget and Timeline 122](#project-budget-and-timeline)
>
> [3.9.11 Standards Compliance 122](#standards-compliance)
>
> [3.9.11.1 Report Format 122](#report-format)
>
> [3.9.11.2 Data Naming 122](#data-naming)
>
> [3.9.11.3 Accounting Procedures 123](#accounting-procedures)
>
> [3.9.11.4 Audit Tracing 123](#audit-tracing)
>
> [3.10. Software system attributes 124](#software-system-attributes)
>
> [3.10.1 Reliability 124](#reliability)
>
> [3.10.2 Availability 124](#availability)
>
> [3.10.3 Security 124](#security-1)
>
> [3.10.4. Maintainability 125](#maintainability)
>
> [3.10.5. Portability 126](#portability)

[**4. Supporting information 127**](#supporting-information)

> [4.1 Interview 127](#interview)
>
> [4.1.1 Interview 1 127](#interview-1)
>
> [4.1.1.1 Interview Preparation 127](#interview-preparation)
>
> [4.1.1.2 Interview Agenda 127](#interview-agenda)
>
> [4.1.1.3 Proof 129](#proof)
>
> [4.1.2 Interview 2 129](#interview-2)
>
> [4.1.2.1 Interview Preparation 129](#interview-preparation-1)
>
> [4.1.1.2 Interview Agenda 129](#interview-agenda-1)
>
> [4.1.2.3 Proof 131](#proof-1)
>
> [4.1.3 Interview 3 131](#interview-3)
>
> [4.1.3.1 Interview Preparation 131](#interview-preparation-2)
>
> [4.1.3.2 Interview Agenda 132](#interview-agenda-2)
>
> [4.1.3.3 Proof 133](#proof-2)
>
> [4.2. Survey 134](#survey)
>
> [4.2.1 Students 134](#students)
>
> [4.2.2 Parents 138](#parents)
>
> [4.3 Observation 143](#observation)
>
> [4.3.1 CliC 143](#clic)
>
> [4.3.2 eBwise 146](#ebwise)

[**5. Verification 149**](#verification)

> [5.1. Verification of External Interfaces (3.2)
> 149](#verification-of-external-interfaces-3.2)
>
> [5.1.1 University Database Interface (3.2.1)
> 149](#university-database-interface-3.2.1)
>
> [5.1.2 Campus Management System (CLiC) Interface (3.2.2)
> 149](#campus-management-system-clic-interface-3.2.2)
>
> [5.1.3 Learning Management System (eBwise) Interface (3.2.3)
> 149](#learning-management-system-ebwise-interface-3.2.3)
>
> [5.1.4 SMS/Email Notification Gateway (3.2.4)
> 150](#smsemail-notification-gateway-3.2.4)
>
> [5.1.5 Authentication Service (SSO/OAuth) Interface (3.2.5)
> 150](#authentication-service-ssooauth-interface-3.2.5)
>
> [5.1.6 Payment Gateway Interface (3.2.6)
> 150](#payment-gateway-interface-3.2.6)
>
> [5.2 Verification of Functional Requirements
> 151](#verification-of-functional-requirements)
>
> [5.3. Verification of Usability Requirements (3.6)
> 156](#verification-of-usability-requirements-3.6)
>
> [5.3.1 User Interface (3.6.1) 156](#user-interface-3.6.1)
>
> [5.3.2 User Experience (3.6.2) 156](#user-experience-3.6.2)
>
> [5.3.3 Communication (3.6.3) 157](#communication-3.6.3)
>
> [5.3.3 Data Protection (3.6.4) 158](#data-protection-3.6.4)
>
> [5.4. Verification of Performance Requirements (3.5)
> 159](#verification-of-performance-requirements-3.5)
>
> [5.4.1 Static Numerical Requirements (3.5.1)
> 159](#static-numerical-requirements-3.5.1)
>
> [5.4.1 Dynamic Numerical Requirements (3.5.2)
> 160](#dynamic-numerical-requirements-3.5.2)
>
> [5.5. Verification of Logical Database Requirements (3.8)
> 162](#verification-of-logical-database-requirements-3.8)
>
> [5.5.1 Data Integrity Enforcement 162](#data-integrity-enforcement)
>
> [5.5.2 Referential Integrity Checks
> 162](#referential-integrity-checks)
>
> [5.5.3 Normalization Compliance 163](#normalization-compliance)
>
> [5.5.4 Query Accuracy and Performance
> 163](#query-accuracy-and-performance)
>
> [5.5.5 Data Redundancy Detection 163](#data-redundancy-detection)
>
> [5.5.6 Transactional Consistency (ACID Properties)
> 163](#transactional-consistency-acid-properties)
>
> [5.5.7 Backup and Recovery Validation
> 164](#backup-and-recovery-validation)
>
> [5.6. Verification of Design Constraints (3.9)
> 164](#verification-of-design-constraints-3.9)
>
> [5.6.1 Compliance with Data Privacy Regulations (3.9.1)
> 164](#compliance-with-data-privacy-regulations-3.9.1)
>
> [5.6.2 Integration with Existing University Systems (3.9.2)
> 164](#integration-with-existing-university-systems-3.9.2)
>
> [5.6.3 Security Standards (3.9.3) 164](#security-standards-3.9.3)
>
> [5.6.4 Accessibility Requirements (3.9.4)
> 165](#accessibility-requirements-3.9.4)
>
> [5.6.5 API Usage Limitations (3.9.5)
> 165](#api-usage-limitations-3.9.5)
>
> [5.6.6 Performance and Scalability (3.9.6)
> 165](#performance-and-scalability-3.9.6)
>
> [5.6.7 User Experience Consistency (3.9.7)
> 165](#user-experience-consistency-3.9.7)
>
> [5.6.8 Data Interoperability (3.9.8)
> 166](#data-interoperability-3.9.8)
>
> [5.6.9 Legal and Ethical Considerations (3.9.9)
> 166](#legal-and-ethical-considerations-3.9.9)
>
> [5.6.10 Project Budget and Timeline (3.9.10)
> 166](#project-budget-and-timeline-3.9.10)
>
> [5.7 Verification of Software System Attributes (3.10)
> 167](#verification-of-software-system-attributes-3.10)

[**6. Appendices 169**](#appendices)

> [6.1 Assumptions and dependencies 169](#assumptions-and-dependencies)
>
> [6.2 Acronyms and abbreviations 170](#acronyms-and-abbreviations)
>
> [6.3 Glossary 171](#glossary)

#

# Introduction

## 1.1 Purpose

The purpose of the software to be developed, known as University
Communication and Services Portal (UCSP) is mainly to provide a
centralized platform for students, parents, lecturers, and
administrators to access academic and administrative information in a
transparent and timely manner. This system aims to integrate seamlessly
with the university's existing Campus Management System (CLiC) to
deliver real-time access to essential data, including academic
performance, attendance records, billing, and fee information.
Ultimately, the portal will ensure effective and timely communication by
integrating an SMS Gateway, allowing automated alerts and notifications
to be sent directly to students and parents. The UCSP will also provide
access to various online tools and services such as student records,
course registration, library resources, and IT support such as
streamlining processes, improving efficiency, and saving time for all
users.

## 1.2 Scope

The software product to be developed is the **University Communication
and Services Portal**, a centralized platform that integrates with
existing university systems such as the Learning Management System
(LMS), academic calendar, and Campus Management System (CMS). This
portal aims to streamline communication and academic service delivery
for students, parents, lecturers, and administrative staff.

The portal will allow students to check grades, attendance, schedules,
register for courses, and pay tuition fees. Parents will be able to
monitor their child's academic performance, receive fee reminders, and
get SMS alerts on important issues. Lecturers can upload grades, mark
attendance, and post course updates, while administrators will manage
user access and system configurations.

Key features include real-time SMS alerts for low attendance and unpaid
fees, automation of routine tasks, and centralized access to academic
notifications and services. The portal is designed to reduce manual
workload, support timely communication, and enhance user engagement
across all roles.

This software aligns with the overall goal of improving communication
flow, increasing operational efficiency, and encouraging student
accountability. By consolidating key academic functions into a single
platform, the portal will deliver greater transparency, faster
information sharing, and improved access to university services for all
stakeholders.

## 1.3 Product overview

### 1.3.1 Product perspective

The University Communication and Services Portal, an integrated academic
management and communication system, plays a central role within the
university's digital ecosystem. It connects multiple internal systems
such as the Campus Management System (CMS), Learning Management System
(LMS), academic calendar, and university database, serving as a unified
access point for students, parents, lecturers, and administrative staff.
Through its integration with services like SMS gateways and email
servers, the portal ensures seamless delivery of notifications,
reminders, and academic information across all user groups.

The portal operates within a broader institutional infrastructure that
includes tools for grading, attendance tracking, course registration,
and financial management. Its functionality overlaps with these systems
by enabling automated data exchange and reducing reliance on manual
processes. For instance, it retrieves student records and schedules from
the CMS, syncs course data with the LMS, and pulls academic deadlines
from the academic calendar system. It also allows parents to access
academic information about their children and receive SMS alerts for
issues like low attendance or unpaid tuition fees.

The portal interfaces with the larger system landscape through several
key connections:

1.  System Interfaces: Integration with CMS, LMS, SMS Gateway, and
    authentication services for real-time data synchronization.

2.  User Interfaces: Intuitive web and mobile interfaces for students,
    parents, lecturers, and administrators.

3.  Hardware Interfaces: Accessible on desktops, smartphones, and
    tablets to support anytime, anywhere use.

4.  Software Interfaces: Seamless connections with internal software
    (academic modules, student database) and external services
    (SMS/email systems).

5.  Communication Interfaces: Reliable protocols for sending and
    receiving automated alerts, reminders, and academic announcements.

At the core of the system is a centralized backend that manages user
access, notifications, and academic workflows. Modules such as
Attendance Management, Course Registration, Grade Upload, and
Announcement Delivery are orchestrated through an internal scheduler and
database engine. These components interact with each other and with
external systems to ensure that users receive accurate, timely, and
personalized information, ultimately reducing administrative burden and
improving engagement.

Figure 1.3.1.1 illustrates the system's context diagram, highlighting
the key external entities that interact with the EduAxis platform.

![](media/image70.png){width="6.5in" height="4.791666666666667in"}

_Figure 1.3.1.1: Context Diagram of the EduAxis platform_

#### 1.3.1.1 System interfaces

**1. Authentication Service Interface**

Functionality: Enables secure user login and role-based access control.

Interface Description: OAuth2-compliant API for verifying credentials
and managing user sessions.

Constraints/Standards: Must support multi-factor authentication (MFA)
and integrate with institutional single sign-on (SSO) services.

Data Flow: Bidirectional -- users send credentials; server returns
access tokens or denial.

**2. Campus Management System Interface**

Functionality: Provides academic records, enrollment data, and tuition
details.

Interface Description: RESTful API to retrieve and update course
registrations, grades, schedules, and financial records.

Constraints: Requires secure HTTPS communication, JSON data format, and
role-based access.

Dependency: Real-time updates from this system are essential for
accurate student dashboards and administrative tools.

**3. University Database Interface**

Functionality: Acts as the central data store for user profiles,
academic histories, payment records, and access logs.

Interface Description: Structured API endpoints for CRUD (Create, Read,
Update, Delete) operations on academic and personal data.

Constraints: Must comply with university data privacy regulations (e.g.,
GDPR, PDPA).

Data Flow: Bidirectional -- supports user-initiated updates and
system-initiated queries.

**4. Learning Management System (LMS) Interface**

Functionality: Syncs coursework, submissions, grades, and lecturer
feedback.

Interface Description: RESTful API to access course materials, manage
assessments, and update student performance data.

Constraints: Requires LMS-compatible data structure and secure
token-based access.

**5. SMS/Email Gateway Interface**

Functionality: Facilitates communication via SMS and email alerts.

Interface Description: External messaging service (e.g., Twilio,
SendGrid) integration for sending real-time alerts and notifications.

Constraints: Must support high availability and comply with
opt-in/opt-out notification policies.

**6. CMS Integration Interface (Content Management System)**

Functionality: Allows admin to post global announcements and update web
content.

Interface Description: Headless CMS API integration (e.g., Strapi or
Contentful) for publishing dynamic content to the portal.

Constraints: Requires real-time syncing and admin authentication tokens.

**7. Helpdesk & Support Ticketing Interface**

Functionality: Manages support requests from students, lecturers, and
administrators.

Interface Description: Internal ticketing system or integration with
services like Freshdesk/Zendesk via APIs.

Constraints: Should support status tracking, prioritization, and
role-based ticket visibility.

**8. User Interface (Human-System Interface)**

Functionality: Provides a responsive, role-sensitive web/mobile UI for
all users.

Interface Description: Web-based interface designed with accessibility
and usability in mind; supports keyboard navigation, screen readers, and
WCAG 2.1 compliance.

Constraints: Optimized for mobile and desktop access; must adapt to the
roles (Student, Parent, Lecturer, Admin) with corresponding permissions
and menus.

**9. Notification Preference Management Interface**

Functionality: Allows users to customize communication preferences.

Interface Description: UI component linked with SMS/Email Gateway APIs
for toggling notification channels (email/SMS/app).

####

#### 1.3.1.2 User interfaces

####

1.  **Student Dashboard**

> The student dashboard serves as the centralized interface to manage
> academic and administrative activities. This dashboard integrates with
> LMS and CMS for real-time updates on grades and coursework progress.
> Students of the university can securely log in and access the
> personalized information as listed below.

- Class schedule, registered courses, and academic calendar

- Academic performance such as grades and attendance records

- Tuition payment status and history

- Notification and alerts including for low attendance and unpaid fees

- Coursework submission status and feedback from lecturers

- Announcement and academic updates

- Profile settings to update student's personal details and notification
  preferences

2.  **Parent Dashboard**

> This dashboard is optimised for concise overviews and direct alerts to
> ensure parents stay informed without overwhelming detail. Parents and
> guardians can log in via a secure portal to monitor their child's
> academic progress. The key features are listed below.

- Viewing the child's grades and attendance status

- Access to course schedule and academic summary

- Notifications for critical issues such as low attendance and
  outstanding fees

- Customizable SMS/email alert preferences

3.  **Lecturer Dashboard**

> Lecturers have access to a role-based dashboard to support teaching
> and communication tasks. This dashboard integrates with LMS to handle
> assignments and grade synchronization seamlessly. This dashboard
> allows lecturers to perform the tasks or actions as listed below.

- Uploading and updating student grades

- Marking and tracking student attendance

- Posting class announcement and updates

- Viewing academic calendar and teaching schedules

- Monitoring overall student performance and participation

4.  **Administrative Control Panel**

> Administrators use a centralized control panel to manage the portal's
> operations and configurations. Key interface features for this control
> panel are listed below.

- User account management for students, lecturers and parents

- System integration tools for syncing with CMS, LMS and notification
  systems

- Workflow automation configuration for fee reminders, grade processing,
  etc.

- Moderation of global announcements and academic communications

- Help Desk ticket management and issue response tracking

- Notification services setup for SMS/email gateway settings

- Access control and data privacy configurations

- Display logs and dashboards for tracking system usage and engagement

5.  **Notification and Alerts Console (Admin-side and
    System-triggered)**

> This module manages and monitors all automated notifications sent by
> the system. In this console Admins can perform the following actions.

- Configure and test SMS/email templates

- View history of alerts triggered by attendance drops, unpaid fees, or
  grade releases

- Set thresholds and conditions for alert generation

- Monitor system queue via the notification scheduler module

6.  **Helpdesk Support Interface**

> Both users and admin will have access to helpdesk interfaces where
> they can perform the following tasks as listed below.

- Students, parents, and lecturers can submit support tickets

- Admins can respond, update, and close tickets via the dashboard

- The interface includes status tracking, ticket history, and response
  logs

#### 1.3.1.3 Hardware interfaces

1.  **Device Compatibility**

> The University Communication and Services Portal is designed to be
> accessible across multiple device types of hardware requirements.
> Those devices include desktop and laptop computers running Windows,
> macOS or Linux operating systems with standard web browser such as
> Chrome, Microsoft, and Google.The portal also supports mobile devices,
> with fully responsive design optimized for Android and iOS smartphones
> and tablets, that enables student, parents and lecturers to access
> information conveniently at any circumstances.. Having multi-device
> compatibility ensures users can engage with the platform efficiently,
> enhancing user experience itself.

2.  **Internet Connectivity**

> Reliable internet connectivity is pivotal for components in the
> University Communication and Service Portal, it facilitates real-time
> updates on communication and data synchronization with the
> university's backend systems. To secure a seamless experience, the
> portal will require a minimum bandwidth of 1 Mbps for basic access and
> 5 Mbps or higher for maximum performance during heavy traffic. The
> system supports both ethernet and Wi-Fi networks, with integration
> into university-managed wifi to provide stable access for users within
> campus. Additionally, the system also supports cloud based access to
> enable off-campus usage with real-time data availability and
> synchronization in all locations. This potent structure will ensure
> fast, engaging communication between the portal and users.

3.  **Data Storage**

> To accommodate large numbers of academic and administrative data, the
> University Communication and Services Portal relies on robust storage
> solutions that include both cloud storage and the university's local
> storage framework. The cloud-based storage serves as the primary
> repository for students\' records, attendance, grades and course
> materials, and offers scalable and secured data management.
> Concurrently, critical data is mirrored on local servers within the
> university's data center, to ensure quick recovery and backup during
> connectivity issues or system failures. The dual-layered approach of
> cloud and local storage ensures that the system remains secured, and
> capable of handling high data loads while maintaining real time
> synchronization with all users.

####

#### 1.3.1.4 Software interfaces

####

1.  **Database Management System (DBMS)**

- Name: PostgreSQL

- Mnemonic: DBMS

- Specification Number: N/A

- Version Number: Latest stable release (PostgreSQL 15+)

- Source: PostgreSQL Global Development Group (Open Source)

- Interface Purpose: The DBMS stores all user data, including student
  profiles, grades, attendance, notification preferences, payment
  records, helpdesk tickets, and system logs. It supports relational
  queries for internal modules and secure transactions during academic
  workflows.

2.  **Web Server**

- Name: NGINX

- Mnemonic: Web Server

- Specification Number: N/A

- Version Number: Latest stable version

- Source: F5 NGINX (Open Source)

- Interface Purpose: The web server hosts the university portal web
  application. It serves the frontend content and routes HTTP(S)
  requests to the backend application. It also acts as a reverse proxy
  API handling and SSL termination.

3.  **Backend Framework**

- Name: Django

- Mnemonic: Backend

- Specification Number: N/A

- Version Number: Django 4.x (Latest LTS)

- Source: Django Software Foundation (Open Source)

- Interface Purpose: The backend framework implements core business
  logic of the portal, including user authentication, data processing,
  internal workflows such as grading and registration, and integration
  points to external systems such as LMS, CMS and SMS gateway.

4.  **Messaging Protocol**

- Name: RESTful API (Representational State Transfer)

- Mnemonic: REST API

- Specification Number: RFC 7231

- Version Number: N/A

- Source: Internet Engineering Task Force (IETF)

- Interface Purpose: This protocol defines the HTTP-based protocol used
  to exchange data between the portal and the external systems like the
  CMS, LMS, SMS Gateway, and Payment Gateway. This follows REST
  conventions for GET, POST, PUT, DELETE operations.

5.  **External Authentication Service**

- Name: OAuth 2.0 / SSO via Central Auth

- Mnemonic: Auth Service

- Specification Number: RFC 6749

- Version Number: Depends on university infrastructure

- Source: University IT Dept / External Identity Provider

- Interface Purpose: The service is used during login to verify user
  identity via centralized authentication, typically integrated with
  campus-wide Single Sign-On systems. Ensures secure and role-based
  access to the portal.

6.  **SMS/Email Notification Gateway**

- Name: Twilio / SMTP

- Mnemonic: Notification Service

- Specification Number: N/A

- Version Number: Latest supported API

- Source: Twilio Cloud API / Mail Server

- Interface Purpose: This gateway sends real-time alerts and reminders
  via SMS and email to students, parents, and lecturers. Triggered by
  internal events such as low attendance, fee due which is configured
  through the admin dashboard.

7.  **Learning Management System (LMS) Integration**

- Name: eBwise (Moodle LMS)

- Mnemonic: LMS

- Specification Number: N/A

- Version Number: As per campus deployment

- Source: University e-learning platform

- Interface Purpose: This integration allows seamless interaction with
  learning materials and assignment submissions. Students and lecturers
  can access coursework links, grade sync, and feedback exchange via
  API-based integration.

8.  **Campus Management System (CMS) Integration**

- Name: Campus Lifecycle Management System (CLiC)

- Mnemonic: CMS

- Specification Number: Internal

- Version Number: Depends on campus deployment

- Source: University Academic System

- Interface Purpose: This integration supplies academic data such as
  grades, attendance records, and billing info. This allows the portal
  to fetch verified academic records for display to students, parents,
  and lecturers.

9.  **Payment Gateway**

- Name: iPay88 / Stripe / FPX Gateway

- Mnemonic: Payment API

- Specification Number: Depends on payment provider

- Version Number: Latest available API

- Source: Third-party payment processor

- Interface Purpose: This gateway handles secure payment processing for
  tuition and fees. This is integrated with the portal for checkout,
  receipt generation, and payment history syncing.

#### 1.3.1.5 Communication Interfaces

**1. HTTP/HTTPS Protocol**

**Purpose**: HTTP/HTTPS is used as the foundational communication
protocol between clients (students, parents, lecturers, admins) and the
university portal's web server. It enables secure transmission of data
during login, course registration, fee payment, and other user-initiated
activities.

**Message Content and Format**:

**Request:** HTTP headers include request methods such as GET, POST,
PUT, and DELETE, along with URLs and optionally a JSON-formatted body
for POST/PUT operations (e.g., submitting feedback or updating
profile).\
**Response:** Includes status codes (e.g., 200 OK, 403 Forbidden),
Content-Type headers (e.g., application/json, text/html), and payloads
(HTML for page rendering, JSON for data APIs).

**2. WebSocket Protocol**

**Purpose**: WebSocket enables real-time, two-way communication between
the portal server and clients for features such as:

- Instant SMS/email alert updates.

- Live helpdesk chat (if implemented).

- Real-time coursework submission statuses or attendance updates.

**Message Content and Format:** Messages use lightweight JSON structures
for real-time updates (e.g., { \"type\": \"notification\", \"message\":
\"Your payment is due.\" }). Binary format may be used for file or
attachment transmissions in coursework or helpdesk uploads.

**3. SMTP Protocol**

**Purpose**: SMTP is used to send automated email messages to users for:

- Account registration and password recovery.

- Course registration confirmations.

- Tuition invoice alerts.

- Announcements and deadlines.

**Message Content and Format**: SMTP messages conform to \[RFC 5321\]
standards and include fields such as:

- From, To, Subject, and Body.

- MIME headers for HTML formatting or file attachments (e.g.,
  application/pdf for fee receipts).

**4. API Integration Protocols**

**Purpose**: REST APIs are employed to interface with external systems:

- Authentication Service for login and session management.

- Campus Management System for accessing grades, fees, and academic
  records.

- Learning Management System (LMS) for coursework and feedback.

- University Database for student and staff data.

**Message Content and Format**: API requests and responses are formatted
in **JSON**, using standard REST methods:

- GET for retrieving data (e.g., academic calendar).

- POST for actions like submitting coursework or feedback.

- PUT for updating profiles.

- DELETE for course withdrawal.

Headers include Authorization (bearer tokens), Content-Type:
application/json, and optional pagination/filtering parameters.

####

####

#### 1.3.1.6 Memory constraints

1\. **Primary Memory (RAM)**

Role: By handling temporary data in the system for quick read and write
during operations RAM is used as the main memory for real-time data
retrieval during users sessions. It manages the application state while
navigating through different modules making smooth and efficient data
retrieval even when handling simultaneous users in the system such as
students, parents, lecturers, and even administrators.

Limitations: The system\'s real-time notification alerts updates require
memory for queueing messages and updating user status. Having high
concurrency during peak periods like course registration and deadlines,
the system will require more RAM for better efficiency in processing
high volume data calls.

2\. **Secondary Memory (Disk Storage)**

Role: Secondary memory in the University Communication and Services
Portal serves as long-term storage for persistent data, including
student records, academic performance logs, attendance data, and
financial transactions. Unlike volatile primary memory (RAM), it retains
data even after system shutdown, ensuring the availability of historical
information and backups.

Limitations: The limitations of secondary memory in the UCSP include
slower read and write speeds compared to primary memory, which can lead
to delays in report generation and registration processes, especially
during peak usage. Its fixed physical capacity can restrict the amount
of historical data that can be stored, making it challenging to maintain
long-term academic records and system logs without regular cleanup or
archiving.

3\. **Caching Mechanism**

Role: The caching mechanism plays a crucial role in improving system
performance and reducing database load by temporarily storing frequently
accessed data. This includes student profiles, academic schedules,
attendance records, and course announcements. By keeping this data in
fast-access memory, the portal can serve requests more quickly without
repeatedly querying the database, leading to faster page loads and
smoother navigation for users.

Limitations: Caching stores data in RAM, which is limited and expensive.
If the cache size grows too large, it can consume critical memory needed
for real-time processes. Furthermore, If the cache is not properly
invalidated or refreshed, users may see outdated information, such as
old grades or attendance records, leading to inconsistencies.

4\. **Session Management**

Role: session management is responsible for maintaining user
authentication and preserving their interactions during a logged-in
session. It enables students, parents, lecturers, and administrators to
securely access their personalized dashboards, view academic records,
perform course registrations, and receive notifications without
repeatedly logging in. Efficient session management ensures data
integrity and prevents unauthorized access by controlling session
timeouts and handling secure data storage.

Limitations: Scalability challenges in managing large numbers of
simultaneous users can consume huge server memory and processing power.
Short session timeouts can also disrupt user experience, while long
timeouts can increase memory consumption and security risk if not
actively managed by any users.

#### 1.3.1.7 Operations

1.  **Modes of Operations:**

- **User initiated Operations:**

  - Users including students, parents, lecturers, and administrators can
    initiate actions such as viewing academic records, uploading grades,
    registering for courses, submitting support tickets, updating
    profiles, and receiving alerts through the portal\'s web-based
    interface.

  - _Students_: View grades, attendance, schedule, make payments, and
    submit coursework.

  - _Lecturers_: Upload grades, post announcements, and mark attendance.

  - _Admins_: Manage users, configure system settings, and monitor
    portal activity.

2.  **Periods of Operations:**

- \*\*Interactive Operations:\*\*
  Users typically interact with the portal during standard academic
  hours (e.g., 8:00 AM -- 10:00 PM). During these hours, all
  functionalities including academic viewing, course registration,
  announcements, and grade management are fully accessible.

- \*\*Unattended Operations:\*\*
  System-level automated processes such as sending scheduled SMS/email
  alerts, updating records from CMS, and executing system health checks
  are conducted during off-peak hours (e.g., overnight) to avoid
  performance disruption.

3.  **Data processing Support Functions**

- **Validation and Integration**:\
  The system validates all user-submitted data (e.g., coursework,
  profile updates) and integrates seamlessly with third-party services
  such as the SMS gateway, authentication provider, and academic
  calendar.

- **Notifications and Alerts**:\
  Automated alerts are generated and dispatched based on data triggers
  (e.g., low attendance or unpaid fees), using background jobs to
  maintain system responsiveness.

- **Reporting and Analytics**:\
  Admin users can generate reports on student performance, attendance
  summaries, and usage metrics to support academic decision-making.

4.  **Backup and Recovery Operations**

- **Regular Backups**:\
  The system performs scheduled backups of essential data including
  student records, grade entries, course schedules, and user accounts.
  Backups are stored securely on cloud infrastructure with redundancy.

- **Disaster Recovery**:\
  In the event of a system failure or data corruption, recovery
  protocols are in place to restore the platform to its last known
  stable state. Recovery time objectives (RTO) are kept minimal to avoid
  academic disruptions.

- **Version Control**:\
  System codebase and configuration changes are managed through version
  control (GitHub), enabling rollback and historical tracking in case of
  issues introduced during updates or new deployments.

####

#### 1.3.1.8 Site adaptation requirements

####

1.  **Data and Initialization Sequences**

> **University-Specific Academic Data:**\
> The system must be adapted to reflect the specific academic structure
> of each university. This includes configuring academic calendars,
> semester start/end dates, registration periods, grading policies,
> course codes, and departmental hierarchies.
>
> **Attendance and Assessment Policies:**\
> The platform should support the initialization of site-specific
> attendance thresholds, warning levels, and performance criteria used
> to trigger alerts or academic risk notifications.
>
> **Payment and Billing Setup:**\
> Initialization sequences must allow customization of tuition
> structures, billing cycles, discount schemes, and payment gateways
> according to the university's financial operations.
>
> **Authentication and Access Control:**\
> Adaptation is required for integration with the university\'s identity
> management system, such as Single Sign-On (SSO), LDAP directories, or
> institutional login portals, to ensure seamless and secure user
> authentication.
>
> **Notification Triggers and Rules:**\
> The system should allow configuration of SMS/email alert rules (e.g.,
> when attendance drops below X%) based on the institution's academic
> and administrative guidelines.

2.  **Site or Mission-Related Features**

> **Custom Branding and UI Customization:**\
> The platform must support university-specific branding, including
> logos, colors, header styles, and portal names, to reflect the
> institution's visual identity.
>
> **Localization and Language Support:**\
> The portal should support localization, including the ability to
> present content in different languages and adapt date/time formats
> based on the region or user preference.
>
> **Campus-Specific Event Configuration:**\
> Site-specific setup is required for configuring academic events,
> holidays, registration dates, and system reminders that align with
> each university's operational calendar.
>
> **SMS Gateway and Communication Setup:**\
> Adaptation is required to integrate with different SMS/email providers
> based on university preference or regional availability. This includes
> setting up API keys, sender IDs, and failover options.
>
> **User Role Configuration and Access Rights:**\
> The platform must support customization of user roles and permissions
> based on the university's structure---for example, allowing certain
> faculties or departments to manage their own announcements or course
> materials.

####

####

####

#### 1.3.1.9 Interfaces with services

1.  \*\*Cloud Hosting Provider\*\*
    The University Communication and Services Portal will be hosted on a
    cloud infrastructure such as Amazon Web Services (AWS) or Google
    Cloud Platform (GCP). These services provide scalable and reliable
    environments for hosting backend services, databases, and
    application logic. The platform will interface with cloud services
    to manage virtual servers, allocate resources, configure networking,
    and ensure system availability through autoscaling, load balancing,
    and backup services. APIs from the hosting provider will be used for
    deployment automation, storage management, and health monitoring.

2.  \*\*SMS Gateway Service\*\*
    To support real-time notifications and alerts (e.g., low attendance,
    unpaid fees), the platform will integrate with a third-party SMS
    gateway service such as Twilio or MessageBird. The system will
    interact with the SMS service via RESTful APIs to send automated
    text messages to students and parents. This integration will allow
    queuing of SMS alerts, tracking delivery status, and managing sender
    identification based on regional requirements. The gateway service
    ensures timely and reliable communication with stakeholders.

3.  \*\*Email Delivery Service\*\*
    The platform will interface with email delivery services such as
    Amazon SES or SendGrid to deliver transactional and system-generated
    emails. These may include grade updates, registration confirmations,
    password resets, and academic announcements. Integration will be
    handled via SMTP or RESTful API calls, enabling the system to manage
    templates, track bounces, monitor open/click rates, and ensure
    compliance with delivery standards. The email service also provides
    logging and analytics for administrative review.

4.  \*\*Authentication and Authorization Services\*\*
    For secure access and user role management, the platform will
    integrate with authentication providers such as Google Identity,
    LDAP, or Microsoft Azure Active Directory. This ensures seamless
    Single Sign-On (SSO) functionality for students, lecturers, and
    administrators. The system will use OAuth 2.0 and OpenID Connect
    protocols to authenticate users, validate tokens, and manage
    role-based access controls (RBAC). APIs will facilitate session
    handling, user profile retrieval, and permission enforcement.

###

### **1.3.2 Product functions**

Figure 1.3.2.1 below shows the generic use case diagram for the
University Communication and Services Portal with Campus Management
System and SMS Gateway Integration.

![](media/image73.png){width="6.5in" height="6.680555555555555in"}

_Figure 1.3.2.1: Generic Use Case Diagram_

Table 1.1 below contains the list of functions to be implemented into
the system which are organized by actors defined for this system.

_Table 1.1: EduAxis Functions_

+--------------+-------------------------------------------------------+
| **Actor** | **Functions** |
+--------------+-------------------------------------------------------+
| Student | 1. Login |
| | |
| | 2. View Academic Grades |
| | |
| | 3. Check Class Attendance Records |
| | |
| | 4. Access/View Course Schedule |
| | |
| | 5. Register/Drop Courses |
| | |
| | 6. Submit Coursework & View Feedback |
| | |
| | 7. Pay Tuition & Other Fees |
| | |
| | 8. View Payment History & Invoices |
| | |
| | 9. Receive SMS/Email Alerts |
| | |
| | 10. View Announcements & Notifications |
| | |
| | 11. Update Personal Profile Information |
| | |
| | 12. Submit Feedback/Support Tickets |
| | |
| | 13. Monitor Student Academic Performance |
| | |
| | 14. Customize Notification Preferences |
+--------------+-------------------------------------------------------+
| Parent | 1. Login |
| | |
| | 2. View Child's Grade & Attendance |
| | |
| | 3. View Child's Payment History & Dues Summary |
| | |
| | 4. Access Child's Schedule & Academic Summary |
| | |
| | 5. View Announcements & Notifications |
| | |
| | 6. Receive SMS/Email Alerts |
| | |
| | 7. Customize Notification Preferences |
+--------------+-------------------------------------------------------+
| Lecturer | 1. Login |
| | |
| | 2. Upload Student Grades |
| | |
| | 3. Manage Coursework Submissions |
| | |
| | 4. Export Grades & Attendance Reports |
| | |
| | 5. Manage Attendance |
| | |
| | 6. View Academic Calendar & Class Schedules |
| | |
| | 7. Post Class Announcements |
| | |
| | 8. Submit Helpdesk Tickets |
+--------------+-------------------------------------------------------+
| Admin | 1. Login |
| | |
| | 2. Manage User Accounts |
| | |
| | 3. Configure & Manage SMS/Email Notification |
| | Services |
| | |
| | 4. Integrate & Sync with CMS, LMS |
| | |
| | 5. Automate Workflows |
| | |
| | 6. Post Global Announcements |
| | |
| | 7. Maintain Data Privacy & Access Permissions |
| | |
| | 8. Respond to Helpdesk Tickets or System Issues |
+==============+=======================================================+

#### 1.3.2.1 Student function

##### 1.3.2.1.1. Login

_Table 1.3.2.1.1. Use case Specification - Login_

+--------------------------+-----------------+----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+-----------------+----------------------------------+
| **ID** | 1.1 | Name | Login |
+----------------+---------+-----------------+----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+-----------------+----------------------------------+
| **Context** | 3.1 | Source | CliC, ebwise |
+----------------+---------+-----------------+----------------------------------+
| **Use Case | 4.1 | Short | The user logs into their account |
| Definition** | | Description | |
| +---------+-----------------+----------------------------------+
| | 4.2 | Goal | Authenticate user identity to |
| | | | access the platform's feature |
| +---------+-----------------+----------------------------------+
| | 4.3 | Actor | Student |
| +---------+-----------------+----------------------------------+
| | 4.4 | Pre-Condition | The user is registered and |
| | | | Authenticated in the system |
| +---------+-----------------+----------------------------------+
| | 4.5 | Post-Condition | The user gains access to |
| | | | personalized features within the |
| | | | system |
| +---------+-----------------+----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | login page. |
| | | | |
| | | | 2\. The user enter their |
| | | | username and password |
| | | | |
| | | | 3\. The user clicks the "Login" |
| | | | button. |
| | | | |
| | | | 4\. The system validates the |
| | | | credentials |
| | | | |
| | | | The system displays the |
| | | | student's dashboard |
| +---------+-----------------+----------------------------------+
| | 4.7 | Alternative | 1\. The user wants to log in |
| | | Scenario | using a social media account |
| | | | such as LinkdIn |
| | | | |
| | | | - The system redirects the user |
| | | | to the social media |
| | | | credentials and authorize |
| | | | access |
| | | | |
| | | | - The user enters their social |
| | | | media credentials and |
| | | | authorize access |
| | | | |
| | | | - The system validates the |
| | | | social media credentials and |
| | | | logs the user in |
| +---------+-----------------+----------------------------------+
| | 4.8 | Exception | 1\. The user enter incorrect |
| | | Scenario | credentials |
| | | | |
| | | | - The system displays an error |
| | | | message indicating invalid |
| | | | credentials |
| | | | |
| | | | - The user is prompted to |
| | | | re-enter their username and |
| | | | password. |
+================+=========+=================+==================================+

![](media/image72.png){width="3.59375in" height="3.1499693788276466in"}

_Figure 1.3.2.1.1. Activity Diagram - Login_

##### 1.3.2.1.2. View Academic Grades

_Table 1.3.2.1.2. Use case Specification - View Academic Grades_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | View academic grades |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CliC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The student views their academic |
| Definition** | | Description | grades through the platform. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Allow students to access and |
| | | | review their academic performance |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The student is logged into the |
| | | | system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | The student displays the |
| | | | student's academic grades |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The students logs into the |
| | | Scenario | system. |
| | | | |
| | | | 2\. The student navigates to the |
| | | | "Grades" section. |
| | | | |
| | | | 3\. The system retrieves the |
| | | | student's grade records. |
| | | | |
| | | | 4\. The grades are displayed on |
| | | | the dashboard. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. No grades data available |
| | | Scenario | |
| | | | - The system display a message: |
| | | | "No grades found." |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. System error during grade |
| | | Scenario | retrieval |
| | | | |
| | | | - An error message is shown: |
| | | | "Unable to load grades. Please |
| | | | try again later." |
+================+=========+================+===================================+

![](media/image75.png){width="3.971493875765529in"
height="5.636017060367454in"}

_Figure 1.3.2.1.2. Activity Diagram - View Academic Grades_

##### 1.3.2.1.3. Check Class Attendance Records

_Table 1.3.2.1.3. Use case Specification - Check Class Attendance
Records_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Check Class Attendance Records |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The student views their |
| Definition** | | Description | attendance records percentage for |
| | | | all enrolled courses |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | To allow students to track their |
| | | | class attendance and stay |
| | | | informed |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The student is successfully |
| | | | logged into the portal. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | The system displays the student's |
| | | | attendance summary for each |
| | | | course. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The student logs into the |
| | | Scenario | system. |
| | | | |
| | | | 2\. The student navigates to the |
| | | | "Attendance" section. |
| | | | |
| | | | 3\. The system retrieves |
| | | | attendance data for the student. |
| | | | |
| | | | 4\. The student views their |
| | | | attendance percentage and record. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. The student has not attended |
| | | Scenario | any classes yet |
| | | | |
| | | | - The system displays "No |
| | | | attendance record available." |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. System fails to retrieve data |
| | | Scenario | |
| | | | - The system displays an error |
| | | | message: "Unable to load |
| | | | attendance. Please try again |
| | | | later." |
+================+=========+================+===================================+

![](media/image74.png){width="4.106707130358705in"
height="6.146926946631671in"}

_Figure 1.3.2.1.3. Activity Diagram - Check Class Attendance Records_

#####

##### 1.3.2.1.4. Access and View Course Schedule/Timetable

_Table 1.3.2.1.4. Use case Specification - Access and View Course
Schedule/Timetable_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | View Course Schedule |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student views their course |
| Definition** | | Description | timetable for the current |
| | | | semester. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Provide access to an up-to-date |
| | | | and organized schedule. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Student is logged into the system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Course schedule is displayed |
| | | | successfully |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Students logs in. |
| | | Scenario | |
| | | | 2\. Navigates to "Timetable". |
| | | | |
| | | | 3\. System loads and display |
| | | | schedule. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Student select a different |
| | | Scenario | semester to view. |
| | | | |
| | | | 2\. Schedule data not available |
| | | | |
| | | | - System shows: "Timetable not |
| | | | found." |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. System fails to retrieve data |
| | | Scenario | |
| | | | - The system displays an error |
| | | | message: "Unable to load |
| | | | timetable. Please try again |
| | | | later." |
+================+=========+================+===================================+

![](media/image77.png){width="3.7656255468066493in"
height="5.301013779527559in"}

_Figure 1.3.2.1.4. Activity Diagram - Access and View Course
Schedule/Timetable_

##### 1.3.2.1.5 Register or Drop Courses

_Table 1.3.2.1.5. Use case Specification - Register or Drop Courses_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Register or Drop Courses |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student registers or drops |
| Definition** | | Description | courses for the semester. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Allow students to manage course |
| | | | enrollment. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Registration period is open. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Courses are updated in the |
| | | | student's schedule. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Student logs in. |
| | | Scenario | |
| | | | 2\. Goes to "Enrollment". |
| | | | |
| | | | 3\. Add course to My Planner. |
| | | | |
| | | | 4\. Go to My Planner. |
| | | | |
| | | | 5\. Choose preferred time table |
| | | | for each course. |
| | | | |
| | | | 6\. Confirm enrollment. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. The class is full |
| | | Scenario | |
| | | | - Student can choose other class |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 2\. Student didn't add any course |
| | | Scenario | to My Planner |
| | | | |
| | | | - System will display "please add |
| | | | course first" |
+================+=========+================+===================================+

![](media/image76.png){width="2.576100174978128in"
height="7.088542213473316in"}

_Figure 1.3.2.1.5. Activity Diagram - Register or Drop Courses_

##### 1.3.2.1.6 Submit Coursework and View Feedback

_Table 1.3.2.1.6. Use case Specification - Submit Coursework and View
Feedback_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Submit Coursework and View |
| | | | Feedback |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | ebwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student uploads assignment and |
| Definition** | | Description | views lecturer feedback. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Provide digital submission and |
| | | | feedback viewing function. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Coursework submission is opened |
| | | | by the lecturer |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | File is submitted and feedback is |
| | | | given by the lecturer |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Student logs in |
| | | Scenario | |
| | | | 2\. Select a course |
| | | | |
| | | | 3\. Go to coursework assigned by |
| | | | the lecturer |
| | | | |
| | | | 4\. Uploads file |
| | | | |
| | | | 5\. Confirm submission |
| | | | |
| | | | 6\. View feedback once marked by |
| | | | the lecturer. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Students can upload multiple |
| | | Scenario | files. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. File upload fail - system |
| | | Scenario | shows: "Upload unsuccessful. Try |
| | | | again." |
+================+=========+================+===================================+

![](media/image80.png){width="4.444044181977253in"
height="6.734375546806649in"}

_Figure 1.3.2.1.6. Activity Diagram - Submit Coursework and View
Feedback_

##### 1.3.2.1.7. Pay Tuition and Other Fees

_Table 1.3.2.1.7. Use case Specification - Pay Tuition and Other Fees_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Pay tuition and Fees |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student pays outstanding tuition |
| Definition** | | Description | or miscellaneous fees online. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Enable fast and secure fee |
| | | | payment |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Student has unpaid fees. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Payment is recorded and receipt |
| | | | issued. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Students log in. |
| | | Scenario | |
| | | | 2\. Goes to "Payments". |
| | | | |
| | | | 3\. System shows outstanding |
| | | | bills. |
| | | | |
| | | | 4\. Students select bills that |
| | | | they want to pay. |
| | | | |
| | | | 5\. Enter payment info |
| | | | |
| | | | 6\. Receives confirmation |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Student saves payment info |
| | | Scenario | for later. |
| | | | |
| | | | 2\. No outstanding balance |
| | | | |
| | | | - System show "You have no |
| | | | outstanding balance" |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Payment fails |
| | | Scenario | |
| | | | - System shows: "Transaction |
| | | | declined." |
+================+=========+================+===================================+

![](media/image78.png){width="4.308823272090988in"
height="4.578125546806649in"}

_Figure 1.3.2.1.7. Activity Diagram - Pay Tuition and Other Fees_

##### 1.3.2.1.8. View Payment History and Invoices

_Table 1.3.2.1.8. Use case Specification - View Payment History and
Invoices_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | View Payment History and Invoices |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Cimb bank |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student views list of paid |
| Definition** | | Description | Invoices and receipts |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Help student track financial |
| | | | history. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Students have made payments |
| | | | before. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Payment records are displayed. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Students log in. |
| | | Scenario | |
| | | | 2\. Goes to "Payment History" |
| | | | |
| | | | 3\. Views or downloads invoices |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Filter payment history by |
| | | Scenario | semester. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. No records |
| | | Scenario | |
| | | | - The system shows: "No payment |
| | | | history found." |
+================+=========+================+===================================+

![](media/image79.png){width="4.234375546806649in"
height="4.138928258967629in"}

_Figure 1.3.2.1.8. Activity Diagram - View Payment History and Invoices_

##### 1.3.2.1.9. Receive SMS/Email Alerts

_Table 1.3.2.1.9. Use case Specification - Receive SMS/Email Alerts_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Receive alerts |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student receives automated alerts |
| Definition** | | Description | vias SMS/email |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Notify students of critical |
| | | | academic and financial updates |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Student is registered and |
| | | | notifications are enabled |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Alerts are received in inbox/SMS. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Event trigger (example; low |
| | | Scenario | attendance) |
| | | | |
| | | | 2\. System sends message |
| | | | |
| | | | 3\. Student receives it |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | Students configure alerts and |
| | | Scenario | preferences. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Delivery fails |
| | | Scenario | |
| | | | - System logs error and retries |
+================+=========+================+===================================+

![](media/image81.png){width="4.489583333333333in"
height="3.6235214348206473in"}

_Figure 1.3.2.1.10. Activity Diagram - Receive SMS/Email Alerts_

##### 1.3.2.1.10 View Announcements and Academic Notifications

_Table 1.3.2.1.10. Use case Specification - View Announcements and
Academic Notifications_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | View Announcements |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Ebwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student views posted updates from |
| Definition** | | Description | lecturers/admins |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Ensure student are informed of |
| | | | academic key notices. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Announcements are posted. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Notifications are read. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Students log in. |
| | | Scenario | |
| | | | 2\. Goes to "Announcements". |
| | | | |
| | | | 3\. View list of announcements. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Filters announcements by |
| | | Scenario | course |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. System fails to load |
| | | Scenario | |
| | | | - System shows: "Unable to |
| | | | retrieve announcements." |
+================+=========+================+===================================+

![](media/image82.png){width="3.8177088801399823in"
height="3.737335958005249in"}

_Figure 1.3.2.1.10. Activity DIagram - View Announcements and Academic
Notifications_

##### 1.3.2.1.11 Update Personal Profile Information

_Table 1.3.2.1.11. Use case Specification - Update Personal Profile
Information_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Update profile |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student edits personal |
| Definition** | | Description | information |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Keep student contact details up |
| | | | to date |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Student is logged in. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Updated info is saved in the |
| | | | system. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Student logs in. |
| | | Scenario | |
| | | | 2\. Goes to "Profile" |
| | | | |
| | | | 3\. Edits info. |
| | | | |
| | | | 4\. Clicks "Save". |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | Student cancels changes |
| | | Scenario | |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | Save fails - system shows: |
| | | Scenario | "Update unsuccessful." |
+================+=========+================+===================================+

![](media/image83.png){width="3.807292213473316in"
height="4.6358213035870515in"}

_Figure 1.3.2.1.11. Activity Diagram - Update Personal Profile
Information_

##### 1.3.2.1.12 Submit Feedback/ Support Tickets

_Table 1.3.2.1.12. Use case Specification - Submit Feedback/ Support
Tickets_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Submit Support Ticket |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student submits a complaint or |
| Definition** | | Description | technical support request. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Allow student to report issues |
| | | | and get assistance |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Student has access to the |
| | | | helpdesk module. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Ticket is created and assigned |
| | | | for review. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Students logs in. |
| | | Scenario | |
| | | | 2\. Students goes to |
| | | | "Help/Support". |
| | | | |
| | | | 3\. Students fills out issue |
| | | | form. |
| | | | |
| | | | 4\. Submit a ticket. |
| | | | |
| | | | 5\. Receives confirmation. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Student views past ticket |
| | | Scenario | status. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Submission fails |
| | | Scenario | |
| | | | - System shows: "Unable to submit |
| | | | ticket." |
+================+=========+================+===================================+

![](media/image84.png){width="3.7743153980752404in"
height="4.494792213473316in"}

_Figure 1.3.2.1.12. Activity Diagram - Submit Feedback/ Support Tickets_

##### 1.3.2.1.13 Monitor Student Academic Performance

_Table 1.3.2.1.13. Use case Specification - Monitor Student Academic
Performance_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Monitor Academic Performance |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student views a summary of their |
| Definition** | | Description | academic performance, including |
| | | | grades and attendance. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Enable students to track their |
| | | | academic progress independently. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Academic data (grades, |
| | | | attendance) is available in the |
| | | | system. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Student has reviewed performance |
| | | | data. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Student logs in. |
| | | Scenario | |
| | | | 2\. Navigates to "Academic |
| | | | Dashboard". |
| | | | |
| | | | 3\. Views performance charts and |
| | | | grade summary. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Filters performance by |
| | | Scenario | semester or subject. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Dashboard fails to load. |
| | | Scenario | |
| | | | - System shows: "Unable to |
| | | | display academic performance." |
+================+=========+================+===================================+

####

#### ![](media/image85.png){width="4.213542213473316in" height="3.9651017060367453in"}

_Figure 1.3.2.1.13. Activity Diagram - Monitor Student Academic
Performance_

#####

##### 1.3.2.1.14 Customize Notification Preferences

_Table 1.3.2.1.14 Use case Specification - Customize Notification
Preferences_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Customize Notification |
| | | | Preferences |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Iman Nadhirah |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | MsTeams |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Student selects preferred |
| Definition** | | Description | notification method for academic |
| | | | alerts (SMS, email, or both). |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Allow students to receive alerts |
| | | | in a format that suits their |
| | | | preference. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Student |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Student has login to their |
| | | | account |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Notification preferences are |
| | | | saved and applied. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Student logs in. |
| | | Scenario | |
| | | | 2\. Goes to "Notification |
| | | | Settings". |
| | | | |
| | | | 3\. Selects preferred channel |
| | | | (SMS/email/both). |
| | | | |
| | | | 4\. Save settings. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Different settings for |
| | | Scenario | different alert types (e.g., SMS |
| | | | for fees, email for grades). |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Settings fail to save. |
| | | Scenario | |
| | | | - System shows: "Notification |
| | | | preferences update failed." |
+================+=========+================+===================================+

####

#### ![](media/image86.png){width="4.36904636920385in" height="4.980260279965004in"}

_Figure 1.3.2.1.14. Activity Diagram - Customize Notification
Preferences_

#### 1.3.2.2 Parent function

1.3.2.2.1 Login

_Table 1.3.2.2.1. Use case Specification - Login_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Login |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Suzannah Pancer |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Parent accesses the system using |
| Definition** | | Description | valid login credentials. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | To authenticate and grant parent |
| | | | access to the system. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Parent |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Parent has an active account in |
| | | | the system. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Parent is redirected to the |
| | | | dashboard. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1. Parent navigates to login |
| | | Scenario | page. |
| | | | |
| | | | 2. Enters username and password. |
| | | | |
| | | | 3. Clicks "Login". |
| | | | |
| | | | 4. System authenticates |
| | | | credentials. |
| | | | |
| | | | 5. Dashboard is displayed. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Parent cancels login attempt. |
| | | Scenario | |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Invalid credentials -- system |
| | | Scenario | shows: "Login failed. Please try |
| | | | again." |
+================+=========+================+===================================+

![](media/image87.png){width="5.28125in" height="5.59375in"}

_Figure_ _1.3.2.2.1. Activity Diagram - Login_

1.3.2.2.2 View Child\'s Grades and Attendance

_Table 1.3.2.2.2. Use case Specification - View Child's Grades and
Attendance_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | View Child\'s Grades and |
| | | | Attendance |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Suzannah Pancer |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Parent views their child's |
| Definition** | | Description | academic grades and class |
| | | | attendance. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | To allow parents to monitor |
| | | | student academic performance. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Parent |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Parent is successfully logged |
| | | | into the system. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | The child's grades and attendance |
| | | | records are displayed. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Parent logs in. |
| | | Scenario | |
| | | | 2\. Dashboard is displayed. |
| | | | |
| | | | 3\. Parent selects "Grades & |
| | | | Attendance". |
| | | | |
| | | | 4\. System retrieves and displays |
| | | | grades and attendance. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Parent cancels the request or |
| | | Scenario | navigates away from the page. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. System fails to retrieve data |
| | | Scenario | -- system shows: "Unable to fetch |
| | | | records." |
+================+=========+================+===================================+

####

#### ![](media/image88.png){width="5.166666666666667in" height="5.59375in"}

_Figure 1.3.2.2.2. Activity Diagram - View Child's Grades and
Attendance_

1.3.2.2.3 Receive SMS/Email alerts (e.g. Low Attendance, Financial Dues)

_Table 1.3.2.2.3. Use case Specification - Receive SMS/Email alerts_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Receive Alerts (e.g. Low |
| | | | Attendance, Financial Dues) |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Suzannah Pancer |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Parent receives automatic alerts |
| Definition** | | Description | via SMS or email when child's |
| | | | attendance is low or dues are |
| | | | pending. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | To keep parents informed about |
| | | | critical academic or financial |
| | | | issues concerning their child. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Parent |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Notification preferences are set |
| | | | and contact details are updated. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Parent is notified through |
| | | | SMS/email when predefined alert |
| | | | conditions are triggered. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1. System detects low attendance |
| | | Scenario | or unpaid dues. |
| | | | |
| | | | 2. Alert message is generated. |
| | | | |
| | | | 3. Message is sent to parent\'s |
| | | | registered contact via SMS or |
| | | | email. |
| | | | |
| | | | 4. Parent receives and reads the |
| | | | notification. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Parent has disabled one of |
| | | Scenario | the notification types (e.g., |
| | | | only SMS or only email is |
| | | | active). |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. System fails to send the |
| | | Scenario | alert -- system logs error and |
| | | | retries or prompts admin. |
+================+=========+================+===================================+

![](media/image59.png){width="6.5in" height="5.597222222222222in"}

_Figure 1.3.2.2.3. Activity Diagram - Receive SMS/Email alerts_

1.3.2.2.4 Access Child\'s Schedule and Academic Summary

_Table 1.3.2.2.4. Use case Specification - Access Child\'s Schedule and
Academic Summary_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Access Child\'s Schedule and |
| | | | Academic Summary |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Suzannah Pancer |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Parents view their child\'s class |
| Definition** | | Description | schedule, subjects, and academic |
| | | | performance summaries. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | To enable parents to monitor |
| | | | their child\'s academic plan and |
| | | | performance easily. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Parent |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Parent is logged in and |
| | | | associated with the child's |
| | | | student profile. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Parent successfully views the |
| | | | child's schedule and academic |
| | | | summary on the system. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1. Parent logs into the portal. |
| | | Scenario | |
| | | | 2. Navigates to "Child Schedule" |
| | | | or "Academic Summary" |
| | | | section. |
| | | | |
| | | | 3. System retrieves and displays |
| | | | the child\'s class schedule |
| | | | and summary of academic |
| | | | performance. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. No schedule or summary is |
| | | Scenario | available for the current |
| | | | academic term --- system shows a |
| | | | message. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Data retrieval error --- |
| | | Scenario | system displays "Unable to load |
| | | | schedule/summary. Please try |
| | | | again." |
+================+=========+================+===================================+

![](media/image60.png){width="6.34375in" height="6.145833333333333in"}

_Figure 1.3.2.2.4. Activity Diagram - Access Child\'s Schedule and
Academic Summary_

1.3.2.2.5 Customize Notification Preferences (SMS/email)

_Table 1.3.2.2.5. Use case Specification - Customize Notification
Preferences (SMS/email)_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Customize Notification |
| | | | Preferences (SMS/email) |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Suzannah Pancer |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | MsTeams |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Parent updates their preferred |
| Definition** | | Description | notification method (SMS, email, |
| | | | or both) for alerts. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | To allow parents to control how |
| | | | they receive important alerts |
| | | | regarding their child. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Parent |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Parent is logged in. Notification |
| | | | settings are available in the |
| | | | system. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Notification preferences are |
| | | | successfully updated and saved in |
| | | | the system. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Parent logs into the portal. |
| | | Scenario | |
| | | | 2\. Navigates to the Notification |
| | | | Settings section. |
| | | | |
| | | | 3\. Selects preferred method(s) |
| | | | (SMS, email). |
| | | | |
| | | | 4\. Clicks \"Save Preferences\". |
| | | | |
| | | | 5\. System confirms the changes. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. Parent selects no method --- |
| | | Scenario | system prompts that at least one |
| | | | method must be selected. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Save operation fails --- |
| | | Scenario | system displays: "Failed to |
| | | | update preferences. Please try |
| | | | again." |
+================+=========+================+===================================+

![](media/image61.png){width="2.0208333333333335in"
height="3.5520833333333335in"}

_Figure 1.3.2.2.5. Activity Diagram - Customize Notification Preferences
(SMS/email)_

1.3.2.2.6 View Payment History and Dues Summary

_Table 1.3.2.2.6. Use case Specification - View Payment History and Dues
Summary_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | View Payment History and Dues |
| | | | Summary |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Suzannah Pancer |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | CLiC |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | Parent views the history of past |
| Definition** | | Description | payments and outstanding dues for |
| | | | their child. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | To provide financial transparency |
| | | | and allow timely fee settlements. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Parent |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | Parent is logged in and linked to |
| | | | at least one student. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | System displays up-to-date |
| | | | payment history and current dues |
| | | | summary. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. Parent logs into the portal. |
| | | Scenario | |
| | | | 2\. Navigates to the "Payments" |
| | | | section. |
| | | | |
| | | | 3\. Selects "View History & |
| | | | Dues". |
| | | | |
| | | | 4\. System displays payment |
| | | | transactions and outstanding |
| | | | dues. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. No payments made yet --- |
| | | Scenario | system shows "No transactions |
| | | | found." |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. Payment data retrieval fails |
| | | Scenario | --- system displays: "Unable to |
| | | | fetch payment records." |
+================+=========+================+===================================+

![](media/image62.png){width="5.072916666666667in"
height="7.604166666666667in"}

_Figure Activity Diagram - View Payment History and Dues Summary_

#### 1.3.2.3 Lecturer function

1.3.2.3.1 Login

_Table 1.3.2.3.1 Use case Specification - Login_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Login |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Clic, ebwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user logs into their account |
| Definition** | | Description | |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Authenticate user identity to |
| | | | access the platform's feature |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user is registered and |
| | | | Authenticated in the system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | The user gains access to |
| | | | personalized features within the |
| | | | system |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | login page. |
| | | | |
| | | | 2\. The user enter their username |
| | | | and password |
| | | | |
| | | | 3\. The user clicks the "Login" |
| | | | button. |
| | | | |
| | | | 4\. The system validates the |
| | | | credentials |
| | | | |
| | | | The system displays the student's |
| | | | dashboard |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. The user wants to log in |
| | | Scenario | using a social media account such |
| | | | as LinkdIn |
| | | | |
| | | | - The system redirects the user |
| | | | to the social media credentials |
| | | | and authorize access |
| | | | |
| | | | - The user enters their social |
| | | | media credentials and authorize |
| | | | access |
| | | | |
| | | | - The system validates the social |
| | | | media credentials and logs the |
| | | | user in |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | > 1\. The user enter incorrect |
| | | Scenario | > credentials |
| | | | |
| | | | - The system displays an error |
| | | | message indicating invalid |
| | | | credentials |
| | | | |
| | | | - The user is prompted to |
| | | | re-enter their username and |
| | | | password. |
+================+=========+================+===================================+

####

![](media/image63.png){width="4.166666666666667in"
height="3.6666666666666665in"}

_Figure 1.3.2.3.1 Activity Diagram - Login_

1.3.2.3.2 Upload student grades

_Table 1.3.2.3.2. Use case Specification - Upload student grades_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Upload student grades |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Clic, ebwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user updates grades of |
| Definition** | | Description | student |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Upload and store grades for |
| | | | students to get updates on |
| | | | Academic Transcripts |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user gains access to make |
| | | | updates in system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Updated info is saved in the |
| | | | system. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | Academic records page. |
| | | | |
| | | | 2\. The user enters the course |
| | | | and student ID of students grade |
| | | | to be updated. |
| | | | |
| | | | 3\. Enters grade credited for |
| | | | specific students. |
| | | | |
| | | | 4\. The user clicks the "Confirm" |
| | | | button. |
| | | | |
| | | | 5\. The system validates the |
| | | | details and stores them in the |
| | | | database. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. The user inserts "bulk |
| | | Scenario | updates" and uploads a |
| | | | pre-formatted excel file |
| | | | containing student ID and their |
| | | | corresponding grades. |
| | | | |
| | | | 2\. The system parses the file, |
| | | | validates the data and displays a |
| | | | summary of updates. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | > 1\. The user enter incorrect |
| | | Scenario | > credentials |
| | | | |
| | | | - The system displays an error |
| | | | message indicating invalid |
| | | | credentials |
| | | | |
| | | | - The user is prompted to |
| | | | re-enter the student IDs and |
| | | | grades. |
+================+=========+================+===================================+

![](media/image64.png){width="2.5416666666666665in"
height="4.157711067366579in"}

_Figure 1.3.2.3.2 Activity Diagram - Upload students grade_

1.3.2.3.3 Mark and manage attendance records

_Table 1.3.2.1.3 Use case Specification - Mark and manage attendance
records_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Mark and manage attendance |
| | | | records |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Clic |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user marks and updates |
| Definition** | | Description | students\' attendance in |
| | | | Student's records. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Mark and update students\' class |
| | | | attendance in the system by the |
| | | | end of class. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user gains access to make |
| | | | updates in system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Updated attendance is saved in |
| | | | the system. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | Attendance records page. |
| | | | |
| | | | 2\. The user enters the course ID |
| | | | and time of class for attendance |
| | | | to be taken. |
| | | | |
| | | | 3\. The system generates one-time |
| | | | QR code with session timeout. |
| | | | |
| | | | 4\. The system receives details |
| | | | of student logging into the |
| | | | session. |
| | | | |
| | | | 5\. The system validates the |
| | | | details and stores them in the |
| | | | database. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. The user manually ticks |
| | | Scenario | students within the class |
| | | | according to the list sorted. |
| | | | |
| | | | 2\. After confirmation the user |
| | | | will click "confirm" |
| | | | |
| | | | 3\. Student's Attendance will be |
| | | | updated into the system. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. The student attempts to scan |
| | | Scenario | the Qr code after the session |
| | | | expires. |
| | | | |
| | | | 2\. The system detects teh |
| | | | expired session and displays an " |
| | | | Attendance session expired" error |
| | | | message. |
| | | | |
| | | | 3\. The student's attendance is |
| | | | not recorded, and system logs |
| | | | failed. |
+================+=========+================+===================================+

####

![](media/image65.png){width="4.161458880139983in"
height="5.31849956255468in"}

_Figure 1.3.2.3.3 Activity Diagram - Mark and update student attendance_

1.3.2.3.4 Post class announcements and updates

_Table 1.3.2.1.4 Use case Specification - Post class announcements and
updates_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Post class announcements and |
| | | | updates |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Ebwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user posts announcements or |
| Definition** | | Description | updates in the system for |
| | | | students\' reference. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Students receive and get updates |
| | | | on announcements and updates made |
| | | | by the lecturer. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user gains access to make |
| | | | updates in system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Announcements is passed to all or |
| | | | selected section of students |
| | | | class |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | main page for specific subject or |
| | | | section |
| | | | |
| | | | 2\. Lecturer navigate to |
| | | | announcements section |
| | | | |
| | | | 3\. Include context or |
| | | | announcements to be delivered. |
| | | | |
| | | | 4\. The lecturers selected the |
| | | | recipient and posted an |
| | | | announcement. |
| | | | |
| | | | 5\. The system delivers the |
| | | | announcement via in-portal |
| | | | notification and optionally |
| | | | triggers email of the selected |
| | | | recipients. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. The lecturer attached |
| | | Scenario | unsupported files or with bigger |
| | | | size than the limit. |
| | | | |
| | | | 2\. The system displays an error |
| | | | message. |
+================+=========+================+===================================+

![](media/image66.png){width="3.6770833333333335in"
height="4.916666666666667in"}

_Figure 1.3.2.3.4 Activity Diagram - Post class announcements and
updates_

1.3.2.3.5 View academic calendar and class schedules

_Table 1.3.2.1.5 Use case Specification - View academic calendar and
class schedules_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | View academic calendar and class |
| | | | schedules |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Clic |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user views their academic |
| Definition** | | Description | calendar and class schedule that |
| | | | has been updated |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Lecturers get their own academic |
| | | | calendar printout and arranged |
| | | | class schedule for the semester. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user is gains access to |
| | | | receive updates in system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Views academic calendar and |
| | | | arranged class schedule. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | class schedule page. |
| | | | |
| | | | 2\. The user enters the Term and |
| | | | subject code |
| | | | |
| | | | 3\. The system displays the |
| | | | academic calendar and class |
| | | | schedule that has been set up by |
| | | | administration. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. The user enters invalid |
| | | Scenario | subject code |
| | | | |
| | | | 2\. The system displays \"No |
| | | | schedule found for the selected |
| | | | term and subject\" error message. |
+================+=========+================+===================================+

####

![](media/image67.png){width="3.84375in" height="4.354166666666667in"}

_Figure 1.3.2.3.5 Activity Diagram -View academic calendar and class
schedules_

1.3.2.3.6 Monitor student academic performance

_Table 1.3.2.1.6 Use case Specification - Monitor student academic
performance_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Monitor student academic |
| | | | performance |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Clic, Ebiwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user monitors a list of |
| Definition** | | Description | students\' academic performance |
| | | | grades. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Lecturers gets to oversee |
| | | | students grade |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user gains access to read |
| | | | updates in the system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | View and oversee students grades |
| | | | performance |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | Students records page. |
| | | | |
| | | | 2\. The user enters the student |
| | | | ID or select name from dropdown |
| | | | list |
| | | | |
| | | | 3\. The system retrieves the |
| | | | student\'s academic records |
| | | | |
| | | | 4\. The system displays the data |
| | | | in a structured format |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. The user enters invalid |
| | | Scenario | student ID code |
| | | | |
| | | | 2\. The system displays |
| | | | \"academic records not available |
| | | | for the selected student and |
| | | | term\" error message. |
+================+=========+================+===================================+

![](media/image68.png){width="2.4531255468066493in"
height="4.332113954505687in"}

_Figure 1.3.2.3.6 Activity Diagram -Monitor student academic
performance_

1.3.2.3.7 Export Grades and Attendance Reports

_Table 1.3.2.1.7 Use case Specification - Export Grades and Attendance
Reports_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Export Grades and Attendance |
| | | | Reports |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Clic, Ebwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user generates or downloads |
| Definition** | | Description | records on grades and attendance |
| | | | reports. |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Users are able to get a copy of |
| | | | grades and attendance reports in |
| | | | desired file format for record |
| | | | keeping. |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user gains access to receive |
| | | | updates in system |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Copies of reports are generated. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to the |
| | | Scenario | Attendance records page. |
| | | | |
| | | | 2\. The user selects exports |
| | | | grades and attendance reports |
| | | | |
| | | | 3\. The system retrieves relevant |
| | | | data from the database. |
| | | | |
| | | | 4\. The system generates previews |
| | | | of the report. |
| | | | |
| | | | 5\. The user clicks the "confirm |
| | | | export" button. |
| | | | |
| | | | 6\. System compiles data and |
| | | | prompts users to download the |
| | | | file. |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. The user selects exports |
| | | Scenario | grades and attendance reports |
| | | | |
| | | | 2\. The system retrieves relevant |
| | | | data from the database. |
| | | | |
| | | | 3\. the system displays an |
| | | | \"Export Failed: Unable to |
| | | | retrieve data\" error message. |
+================+=========+================+===================================+

#### ![](media/image11.png){width="2.2427898075240593in" height="4.473958880139983in"}

_Figure 1.3.2.3.7 Activity Diagram -Export grades and attendance
reports_

1.3.2.3.8 Manage Coursework Submissions

_Table 1.3.2.1.8 Use case Specification - Manage Coursework submission_

+--------------------------+----------------+-----------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+-----------------------------------+
| **ID** | 1.1 | Name | Manage coursework submission |
+----------------+---------+----------------+-----------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+-----------------------------------+
| **Context** | 3.1 | Source | Ebwise |
+----------------+---------+----------------+-----------------------------------+
| **Use Case | 4.1 | Short | The user creates, monitor and |
| Definition** | | Description | mark assignments |
| +---------+----------------+-----------------------------------+
| | 4.2 | Goal | Grade student's contribution in |
| | | | the assignment given |
| +---------+----------------+-----------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+-----------------------------------+
| | 4.4 | Pre-Condition | The user gains access to make |
| | | | updates in system. |
| +---------+----------------+-----------------------------------+
| | 4.5 | Post-Condition | Updated grades on coursework |
| | | | assigned. |
| +---------+----------------+-----------------------------------+
| | 4.6 | Main Success | 1\. The user navigates to |
| | | Scenario | Coursework page of chosen class |
| | | | |
| | | | 2\. The lecturer writes and |
| | | | creates assignments |
| | | | specifications. |
| | | | |
| | | | 3\. Coursework posted with a due |
| | | | date set. |
| | | | |
| | | | 4\. The system triggers email or |
| | | | students assigned for the |
| | | | assignment |
| | | | |
| | | | 5\. The lecturer can monitor |
| | | | students who handed in or not. |
| | | | |
| | | | 6\. Give marks or grades |
| | | | respectively to the coursework. |
| +---------+----------------+-----------------------------------+
| | 4.7 | Alternative | 1\. The coursework given does not |
| | | Scenario | have a due date set |
| | | | |
| | | | 2\. System accepts late |
| | | | submissions and flags it as |
| | | | "late". |
| +---------+----------------+-----------------------------------+
| | 4.8 | Exception | 1\. The student attempt to upload |
| | | Scenario | unsupported file type or have |
| | | | disrupted network |
| | | | |
| | | | 2\. System detects the issue and |
| | | | prevents the submission. |
| | | | |
| | | | 3\. Student is prompted to |
| | | | re-upload the file with correct |
| | | | format and strong internet |
| | | | connectivity |
+================+=========+================+===================================+

####

![](media/image12.png){width="5.083333333333333in"
height="6.666666666666667in"}

_Figure 1.3.2.3.8 Activity Diagram -Manage Coursework Submission_

1.3.2.3.9 Submit Helpdesk tickets

_Table 1.3.2.4.9. Use case Specification - Submit helpdesk tickets_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Submit Helpdesk Tickets or System |
| | | | Issues |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Natasha Adilyn |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | Helpdesk & Support Module |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | Lecturer submits form or tickets |
| Definition** | | Description | upon issues faced in the system. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Shares user issues and for future |
| | | | improvements |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Lecturer |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | Support tickets must exist in the |
| | | | system. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | Tickets are resolved, updated, or |
| | | | escalated. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. Lecturer opens the ticket |
| | | Scenario | dashboard. |
| | | | |
| | | | 2. submit new tickets on issues |
| | | | gone through. |
| | | | |
| | | | 3. System validates the form and |
| | | | store in support database |
| | | | |
| | | | 4. System updates admins on ticket |
| | | | issued |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | The system flags for user follow-up |
| | | Scenario | if the ticket is invalid or |
| | | | incomplete. |
+================+=========+================+======================================+

![](media/image13.png){width="3.34375in" height="4.885416666666667in"}

_Figure 1.3.2.3.9 Activity Diagram - Submit helpdesk tickets_

####

#### 1.3.2.4 Administrator function

1.3.2.4.1 Login

_Table 1.3.2.4.1. Use case Specification - Login_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Login |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | EduAxis Portal (Auth integrated with |
| | | | centralized Authentication Service) |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | The user logs in to access |
| Definition** | | Description | personalized features in the EduAxis |
| | | | portal. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Authenticate user identity to access |
| | | | the platform's features. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | The user must be registered and |
| | | | their account must exist in the |
| | | | system. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | The user is granted access to their |
| | | | dashboard and personalized features. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. The user navigates to the login |
| | | Scenario | page. |
| | | | |
| | | | 2. The user enters their username |
| | | | and password. |
| | | | |
| | | | 3. The user clicks the "Login" |
| | | | button. |
| | | | |
| | | | 4. The system authenticates the |
| | | | credentials via the |
| | | | Authentication Service. |
| | | | |
| | | | 5. The system redirects the user to |
| | | | their role-specific dashboard. |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | 1. The user logs in via centralized |
| | | Scenario | university SSO (Single Sign-On). |
| | | | |
| | | | 2. The system redirects to the |
| | | | university SSO login page. |
| | | | |
| | | | 3. The user enters SSO credentials |
| | | | and grants access. |
| | | | |
| | | | 4. The system validates the |
| | | | credentials via Authentication |
| | | | Service. |
| | | | |
| | | | 5. The user is redirected to their |
| | | | portal dashboard. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | 1. The user enters incorrect |
| | | Scenario | credentials. |
| | | | |
| | | | 2. The system shows an error |
| | | | message: "Invalid username or |
| | | | password." |
| | | | |
| | | | 3. The user is prompted to re-enter |
| | | | credentials or reset password. |
+================+=========+================+======================================+

![](media/image14.png){width="3.648742344706912in"
height="3.7968755468066493in"}

_Figure 1.3.2.4.1. Activity Diagram - Login_

1.3.2.4.2 Manage User Accounts

_Table 1.3.2.4.2. Use case Specification - Manage User Accounts_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Manage User Accounts |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | EduAxis Portal -- Admin Module |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | The Admin manages user creation, |
| Definition** | | Description | updates, and deactivation. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Maintain user account lifecycle |
| | | | securely and efficiently. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | Admin must be authenticated with |
| | | | necessary privileges. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | User accounts are added, updated, or |
| | | | removed as required. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. Admin accesses User Management |
| | | Scenario | Panel. |
| | | | |
| | | | 2. Selects Create, Edit, or Delete |
| | | | action. |
| | | | |
| | | | 3. The system updates the |
| | | | University Database accordingly. |
| | | | |
| | | | 4. Success confirmation is |
| | | | displayed. |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | Admin bulk uploads accounts using a |
| | | Scenario | template CSV. |
| | | | |
| | | | System processes and confirms |
| | | | successful imports. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | If user data is invalid or username |
| | | Scenario | exists, the system returns an error |
| | | | for correction. |
+================+=========+================+======================================+

![](media/image15.png){width="4.145833333333333in"
height="4.050086395450569in"}

_Figure 1.3.2.4.2. Activity Diagram - Manage User Accounts_

1.3.2.4.3 Configure & Manage SMS/Email Notification Services

_Table 1.3.2.4.3. Use case Specification - Configure & Manage SMS/Email
Notification Services_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Configure & Manage SMS/Email |
| | | | Notification Services |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | Notification Module, Admin Dashboard |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | Admin configures alert templates and |
| Definition** | | Description | manages sending services. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Ensure effective communication via |
| | | | automated alerts. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | Admin has system settings access and |
| | | | configured gateway credentials. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | Notification templates are saved and |
| | | | services are connected. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. Admin opens Notification |
| | | Scenario | Settings. |
| | | | |
| | | | 2. Edits or adds SMS/email |
| | | | templates. |
| | | | |
| | | | 3. Links with active SMS Gateway. |
| | | | |
| | | | 4. The system confirms and enables |
| | | | service. |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | Admin enables or disables |
| | | Scenario | notifications per user type or alert |
| | | | category. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | Alert and retry option is displayed |
| | | Scenario | when the system fails to connect to |
| | | | the SMS Gateway. |
+================+=========+================+======================================+

![](media/image16.png){width="3.276042213473316in"
height="3.174928915135608in"}

_Figure 1.3.2.4.3. Activity Diagram - Configure & Manage SMS/Email
Notification Services_

1.3.2.4.4 Integrate & Sync with CMS, LMS

_Table 1.3.2.4.4. Use case Specification - Integrate & Sync with CMS,
LMS_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Integrate & Sync with CMS, LMS |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | Integration Settings -- External |
| | | | Systems |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | Admin configures integration with |
| Definition** | | Description | academic & learning systems. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Synchronize data from external |
| | | | systems like grades, attendance, and |
| | | | coursework. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | External system credentials and API |
| | | | endpoints must be configured. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | The system is successfully synced |
| | | | with external CMS or LMS. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. Admin opens the Integration |
| | | Scenario | Panel. |
| | | | |
| | | | 2. Enters LMS/CMS API settings. |
| | | | |
| | | | 3. Initiates sync. |
| | | | |
| | | | 4. The system pulls data and |
| | | | confirms success. |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | Admin sets auto-sync intervals such |
| | | Scenario | as daily at midnight. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | System logs and notifies admin when |
| | | Scenario | sync is failed due to invalid |
| | | | credentials or timeout. |
+================+=========+================+======================================+

![](media/image17.png){width="3.4531255468066493in"
height="3.623649387576553in"}

_Figure 1.3.2.4.4. Activity Diagram - Integrate & Sync with CMS, LMS_

1.3.2.4.5 Automate Workflows

_Table 1.3.2.4.5. Use case Specification - Automate Workflows_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Automate Workflows |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | Workflow Automation Module |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | Admin sets up automation for |
| Definition** | | Description | repetitive tasks like grade |
| | | | processing or fee alerts. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Reduce manual work and ensure timely |
| | | | task execution. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | Trigger conditions and tasks must be |
| | | | defined. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | Workflows are saved and activated. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. Admin creates a new workflow. |
| | | Scenario | |
| | | | 2. Defines trigger conditions such |
| | | | as attendance \< 80%. |
| | | | |
| | | | 3. Assigns actions such as sending |
| | | | alerts. |
| | | | |
| | | | 4. Saves and activates workflow. |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | Admin clones or edits existing |
| | | Scenario | workflows. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | System logs error and disables rule |
| | | Scenario | when workflow fails due to missing |
| | | | rule. |
+================+=========+================+======================================+

![](media/image18.png){width="3.057292213473316in"
height="3.23452646544182in"}

_Figure 1.3.2.4.5. Activity Diagram - Automate Workflows_

1.3.2.4.6 Post Global Announcements

_Table 1.3.2.4.6. Use case Specification - Post Global Announcements_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Post Global Announcements |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | Announcement Module |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | Admin publishes announcements |
| Definition** | | Description | visible to all users. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Broadcast important university-wide |
| | | | messages. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | Admin is logged in and has |
| | | | announcement privileges. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | Announcements are published and |
| | | | visible to the target audience. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. Admin opens the Announcement |
| | | Scenario | Panel. |
| | | | |
| | | | 2. Composes message. |
| | | | |
| | | | 3. Sets audience and schedule. |
| | | | |
| | | | 4. Publishes announcement. |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | Admin schedules the announcement to |
| | | Scenario | auto-publish later. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | System prompts correction when |
| | | Scenario | content validation fails (missing |
| | | | fields). |
+================+=========+================+======================================+

![](media/image19.png){width="3.1041666666666665in"
height="3.692325021872266in"}

_Figure 1.3.2.4.6. Activity Diagram - Post Global Announcements_

1.3.2.4.7 Maintain Data Privacy & Access Permissions

_Table 1.3.2.4.7. Use case Specification - Maintain Data Privacy &
Access Permissions_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Maintain Data Privacy & Access |
| | | | Permissions |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | System Access Control Panel |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | Admin sets access levels and privacy |
| Definition** | | Description | rules for users. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Ensure only authorized users can |
| | | | access sensitive data. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | Roles and permission sets are |
| | | | defined in the system. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | User access levels are enforced and |
| | | | updated. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 1. Admin opens Access Control |
| | | Scenario | Panel. |
| | | | |
| | | | 2. Selects user/role. |
| | | | |
| | | | 3. Assigns or modifies permissions. |
| | | | |
| | | | 4. Saves changes. |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | Admin imports permission templates |
| | | Scenario | by role. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | The system prompts resolution when |
| | | Scenario | conflicting access levels are |
| | | | detected. |
+================+=========+================+======================================+

![](media/image20.png){width="3.280984251968504in"
height="4.039362423447069in"}

_Figure 1.3.2.4.7. Activity Diagram - Maintain Data Privacy & Access
Permissions_

1.3.2.4.8 Respond to Helpdesk Tickets or System Issues

_Table 1.3.2.4.8. Use case Specification - Respond to Helpdesk Tickets
or System Issues_

+--------------------------+----------------+--------------------------------------+
| **No.** | **Section** | **Content** |
+----------------+---------+----------------+--------------------------------------+
| **ID** | 1.1 | Name | Respond to Helpdesk Tickets or |
| | | | System Issues |
+----------------+---------+----------------+--------------------------------------+
| **Management** | 2.1 | Author | Pharthiban A/L Kumarhesan |
+----------------+---------+----------------+--------------------------------------+
| **Context** | 3.1 | Source | Helpdesk & Support Module |
+----------------+---------+----------------+--------------------------------------+
| **Use Case | 4.1 | Short | Admin views and responds to |
| Definition** | | Description | user-submitted support tickets. |
| +---------+----------------+--------------------------------------+
| | 4.2 | Goal | Resolve user issues and improve user |
| | | | satisfaction. |
| +---------+----------------+--------------------------------------+
| | 4.3 | Actor | Admin |
| +---------+----------------+--------------------------------------+
| | 4.4 | Pre-Condition | Support tickets must exist in the |
| | | | system. |
| +---------+----------------+--------------------------------------+
| | 4.5 | Post-Condition | Tickets are resolved, updated, or |
| | | | escalated. |
| +---------+----------------+--------------------------------------+
| | 4.6 | Main Success | 5. Admin opens ticket dashboard. |
| | | Scenario | |
| | | | 6. Views new/unresolved tickets. |
| | | | |
| | | | 7. Assigns and responds. |
| | | | |
| | | | 8. Updates ticket status (closed, |
| | | | escalated, resolved). |
| +---------+----------------+--------------------------------------+
| | 4.7 | Alternative | Admin responds using canned |
| | | Scenario | responses or knowledge base links. |
| +---------+----------------+--------------------------------------+
| | 4.8 | Exception | The system flags for user follow-up |
| | | Scenario | if the ticket is invalid or |
| | | | incomplete. |
+================+=========+================+======================================+

![](media/image1.png){width="3.327491251093613in"
height="3.7552088801399823in"}

_Figure 1.3.2.4.8. Activity Diagram - Respond to Helpdesk Tickets or
System Issues_

### **1.3.3 User Characteristics**

#### 1.3.3.1 Student

**Educational Level**: Undergraduate or postgraduate students enrolled
at the university.

**Experience**: Varies; may include first-year students unfamiliar with
university systems to final-year students with moderate experience using
institutional portals.

**Technical Expertise**: Basic to moderate. Familiar with smartphones,
web platforms, and learning tools but may require intuitive interfaces
for administrative tasks.

**Disabilities**: Some users may have visual, motor, or cognitive
impairments.

**Usability Influence**: Interfaces must be mobile-responsive, easy to
navigate, and include accessibility features such as screen reader
support, color contrast, and simple forms. Timely feedback and
automation are critical for reducing user frustration.

#### 1.3.3.2 Parent or Guardian

**Educational Level**: Varies significantly; may include
non-university-educated users.

**Experience**: Limited or no experience with academic portals;
typically unfamiliar with institutional systems or digital academic
tools.

**Technical Expertise**: Low to moderate. May only access the portal
occasionally via mobile devices.

**Disabilities**: May include older users with visual impairments or
limited digital literacy.

**Usability Influence**: Requires a simple, mobile-friendly interface
with clear language, SMS alerts, and minimal navigation layers. SMS
notification design is critical due to likely preference for mobile
communication over in-portal browsing.

#### 1.3.3.3 Lecturer

**Educational Level**: Postgraduate degree holders with academic or
research backgrounds.

**Experience**: Extensive experience in higher education and academic
administration.

**Technical Expertise**: Moderate to high. Familiar with digital
learning tools, spreadsheets, and content management systems.

**Disabilities**: May include individuals with visual fatigue or
repetitive stress injuries.

**Usability Influence**: Portal features (e.g., attendance marking,
grade uploads, announcements) must be efficient, logically structured,
and integrate seamlessly with existing tools like the LMS. Time-saving
automation and bulk-processing features are essential.

#### 1.3.3.4 Administrator

**Educational Level**: Professional or technical staff with tertiary
education.

**Experience**: High level of familiarity with institutional systems and
administrative protocols.

**Technical Expertise**: High. Skilled in managing data, user
permissions, system configurations, and troubleshooting.

**Disabilities**: May vary; considerations for ergonomic design and
interface responsiveness apply.

**Usability Influence**: Requires robust tools for platform
configuration, user management, and report generation. Interfaces must
support multitasking, advanced filtering/search, and error-handling
mechanisms for administrative operations.

###

### **1.3.4 Limitations**

1.  **Digital Literacy Gaps**

> Parents or guardians with limited access to technical expertise may
> struggle to navigate the portal, especially if its not fully optimized
> for mobile devices like smartphones, with simple and user-friendly
> design. This can lead to difficulties in accessing important academic
> information, receiving notifications and engaging with students\'
> records actively.

2.  **High Concurrent User Loads**

> During peak usage periods such as subject registration or exam results
> announcements, the platform might experience slowdowns or even crashes
> if it is not properly optimized for scalability. High traffic volumes
> can overload servers, causing delays in data retrieval and frustrating
> users who rely on real-time updates.

3.  **Data Synchronization issues**

> The portal relies on real-time integration with the Campus Managements
> System (CMS) and Learning Management System (LMS) to deliver
> up-to-date information. However, synchronisation delays or connection
> issues between these systems can results in outdated or incomplete
> data being displayed, potentially affecting decision making and
> user-trust.

4.  **Security and Privacy Risk**

> Given the sensitive nature of the data managed by the portal, such as
> student grades, attendance records, and financial information, robust
> security measures are crucial. Insufficient protection can lead to
> unauthorized access, data breaches, and privacy violations,
> compromising student confidentiality and institutional trust.

5.  **Manual Data Entry**

> The process of lecturers manually entering grades or marking
> attendance in the database can introduce human errors, such as typos
> or incorrect records. These inaccuracies can affect student academic
> records, leading to disputes and requiring time-consuming corrections
> to maintain data integrity.

##

#

# 2. References

This document is prepared in reference to the following documents:

I. ISO/IEC/IEEE 29148:2018(E) - International Standard

II. Software Requirement Engineering Lecture Slide

#

# 3. Requirements

## 3.1 Apportioning of Requirements

This section outlines the allocation of system requirements to specific
modules within the University Portal System. Each module is structured
to support user-specific functionality for students, parents, lecturers,
and administrators, ensuring efficient and secure operations.

### 3.1.1 Student Module

---

**Requirement **Description\*\* **Related Functions**
ID\*\*

---

S-1 User authentication and Login
authorization

S-2 View academic performance View Academic Grades,
and grades Monitor Student Academic
Performance

S-3 Manage course registration Register/Drop Courses

S-4 View and pay tuition and Pay Tuition & Other Fees,
fees View Payment History &
Dues Summary

S-5 Access and view class Access/View Course
schedules Schedule

S-6 Submit feedback and support Submit Feedback/Support
tickets Tickets

S-7 View announcements and View Announcements &
receive notifications Notifications, Receive
SMS/Email Alerts

S-8 Customize notification Customize Notification
preferences Preferences

---

### 3.1.2 Parent Module

---

**Requirement **Description\*\* **Related Functions**
ID\*\*

---

P-1 Monitor child\'s academic View Child\'s Grade &
and attendance summary Attendance, Access Child's
Schedule

P-2 View payment and dues View Payment History & Dues
summary Summary

P-3 View announcements and View Announcements &
receive alerts Notifications, Receive
SMS/Email Alerts

---

### 3.1.3 Lecturer Module

---

**Requirement ID** **Description** **Related Functions**

---

L-1 Post class announcements Post Class
Announcements

L-2 Upload grades and manage Upload Student Grades,
coursework submissions Manage Coursework
Submissions

L-3 View academic calendar and View Academic Calendar,
manage attendance Manage Attendance

L-4 Export grades and attendance Export Grades &
reports Attendance Reports

L-5 Submit helpdesk tickets Submit Helpdesk Tickets

---

### 3.1.4 Admin Module

---

**Requirement ID** **Description** **Related Functions**

---

A-1 User authentication and Login
authorization

A-2 Manage user accounts and Manage User Accounts,
permissions Maintain Access
Permissions

A-3 Respond to system issues and Respond to Helpdesk
helpdesk tickets Tickets/System Issues

A-4 Manage data privacy Maintain Data Privacy

A-5 Post and manage global Post Global
announcements Announcements

A-6 Configure and manage Configure & Manage
SMS/email services SMS/Email Notification
Services

A-7 Automate system workflows Automate Workflows

A-8 Integrate with CMS and LMS Integrate & Sync with
CMS, LMS

---

##

## 3.2 External interfaces

### 3.2.1 University Database Interface

---

**Name of Item** University Database Interface

---

**Description of To store and retrieve student, lecturer, parent,
Purpose** and admin data, including profiles, access
permissions, academic history, preferences, and
support tickets.

**Source of University central PostgreSQL database
Input/Destination of  
 Output**

**Valid Range, High accuracy; only verified and registered user
Accuracy, and/or and academic records are stored.
Tolerance**

**Units of Measure** N/A

**Timing** On-demand queries and periodic backups/sync jobs

**Relationships to Used by authentication, user management,
Other academic, and helpdesk modules
Inputs/Outputs**

**Data Formats** JSON

**Command Formats** RESTful API requests (GET, POST, PUT, DELETE)

**Data Items User profiles, grades, attendance, preferences,
Included** ticket logs

**Author** Pharthiban A/L Kumarhesan

---

### 3.2.2 Campus Management System (CLiC) Interface

---

**Name of Item** CMS (Campus Management System) Integration

---

**Description of To fetch verified academic records including
Purpose** grades, billing, attendance from the campus ERP
(CLiC) system.

**Source of CLiC (Campus ERP) System
Input/Destination of  
 Output**

**Valid Range, Verified academic data; matches
Accuracy, and/or registrar-approved records
Tolerance**

**Units of Measure** Grades (GPA/Percentage), Attendance (%)

**Timing** Scheduled sync (nightly), or on-demand trigger

**Relationships to Supplies data to student, lecturer, and parent
Other dashboards
Inputs/Outputs**

**Data Formats** JSON

**Command Formats** RESTful API requests (GET, POST) with token auth

**Data Items Grades, attendance, course registration info, fee
Included** status

**Author** Pharthiban A/L Kumarhesan

---

### 3.2.3 Learning Management System (LMS) Interface

---

**Name of Item** LMS (Moodle/eBwise) Interface

---

**Description of To synchronize assignment submissions, course
Purpose** materials, and grade uploads between the portal
and the LMS.

**Source of University LMS
Input/Destination of  
 Output**

**Valid Range, High accuracy; syncs with instructor-uploaded
Accuracy, and/or data
Tolerance**

**Units of Measure** Submission timestamps, file count, grade values

**Timing** On-demand or triggered during submission events

**Relationships to Connects student and lecturer dashboard to LMS
Other coursework
Inputs/Outputs**

**Data Formats** JSON

**Command Formats** RESTful API (GET, POST, PUT)

**Data Items Assignment files, feedback, grades, course links
Included**

**Author** Pharthiban A/L Kumarhesan

---

### 3.2.4 SMS & Email Gateway Interface

---

**Name of Item** Notification Gateway Integration

---

**Description of To send automated SMS and email alerts related to
Purpose** grades, attendance, fee dues, announcements, and
helpdesk updates.

**Source of SMS/Email Gateway Provider (Twilio, SMTP service)
Input/Destination of  
 Output**

**Valid Range, Requires verified phone/email addresses; delivery
Accuracy, and/or statuses tracked
Tolerance**

**Units of Measure** Message status (sent, failed), timestamp

**Timing** Trigger-based (event-driven notifications)

**Relationships to Triggered by workflows in notification module
Other  
 Inputs/Outputs**

**Data Formats** JSON, SMTP Text

**Command Formats** HTTP POST for API-based SMS, SMTP for emails

**Data Items Recipient info, message content, timestamp,
Included** delivery status

**Author** Pharthiban A/L Kumarhesan

---

### 3.2.5 Authentication Service Interface

---

**Name of Item** Central Authentication Service

---

**Description of To authenticate portal users using centralized
Purpose** university login credentials (such as SSO).

**Source of University SSO system or OAuth 2.0 provider
Input/Destination of  
 Output**

**Valid Range, Auth tokens must be valid and unexpired
Accuracy, and/or  
 Tolerance**

**Units of Measure** Token expiry (minutes), login attempts

**Timing** On every login session

**Relationships to Connects to portal login form and session manager
Other  
 Inputs/Outputs**

**Data Formats** JSON

**Command Formats** OAuth 2.0 (POST, Token Exchange), SAML, or JWT

**Data Items User ID, access token, session info
Included**

**Author** Pharthiban A/L Kumarhesan

---

### 3.2.6 Payment Gateway Interface

---

**Name of Item** Online Payment Gateway

---

**Description of To process tuition and other fee payments
Purpose** securely from students and/or parents.

**Source of Payment provider (such as FPX, Stripe, iPay88)
Input/Destination of  
 Output**

**Valid Range, Amounts must match invoice records; high
Accuracy, and/or transactional accuracy
Tolerance**

**Units of Measure** Amount (MYR), transaction ID

**Timing** Triggered on user-initiated payment

**Relationships to Connects to student dashboard and university
Other accounting system
Inputs/Outputs**

**Data Formats** JSON

**Command Formats** RESTful API (POST, GET)

**Data Items Payment ID, invoice ID, status, timestamp, amount
Included**

**Author** Pharthiban A/L Kumarhesan

---

## 3.3 Elicitation Techniques Based on Kano Model

The requirements for the University Communication and Services Portal
were gathered and prioritized using the Kano Model, which helps in
understanding and categorizing customer needs. The Kano Model
categorizes requirements into five categories:

1.  **Dissatisfier (Must-Be Requirements)**: Basic features that users
    expect. If these are not fulfilled, users will be dissatisfied.

2.  **Satisfier (One-Dimensional Requirements):** Features that result
    in satisfaction when fulfilled and dissatisfaction when not
    fulfilled.

3.  **Delighter (Attractive Requirements):** Features that delight users
    when fulfilled but do not cause dissatisfaction when not fulfilled.

_Table 3.3.1 Prioritization Categories of Functional Requirements_

+-------------------+--------------------------------------------------+
| **Prioritization | **Requirements** |
| Categories** | |
+-------------------+--------------------------------------------------+
| Dissatisfier | 1. User authentication and Authorization |
| | |
| | 2. View academic Grades |
| | |
| | 3. Access Attendance Records |
| | |
| | 4. Access Academic Timetable |
| | |
| | 5. Manage User Accounts and Roles |
| | |
| | 6. Integration with Campus System |
| | (CMS,LMS,Calendar) |
| | |
| | 7. Maintain Data Privacy and Access Permissions |
| | |
| | 8. Pay Tuition and Other Fees |
| | |
| | 9. View Payment History and Invoices |
+-------------------+--------------------------------------------------+
| Satisfier | 1. Upload and Manage Grades |
| | |
| | 2. Digital Attendance Tracking |
| | |
| | 3. Post Announcement and Updates |
| | |
| | 4. Dashboard with Performance Overview |
| | |
| | 5. Submit Feedback and Support Requests |
| | |
| | 6. Alert and Reminder System |
+-------------------+--------------------------------------------------+
| Delighter | 1. Notification Read Tracking |
| | |
| | 2. Custom Notification Preferences |
| | |
| | 3. Visual Performance Analytics |
| | |
| | 4. Mobile-Friendly Responsive Interface |
+===================+==================================================+

_Table 3.3.2 Timeline for Software Requirements Specification of EduAxis
platform_

+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| **Weeks** |
+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+
| **1** | **2** | **3** | **4** | **5** | **6** | **7** | **8** | **9** | **10** | **11** | **12** |
+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+
| Preliminary | | | | | | | | | |
+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+
| | | Elicitation Planning | | | | | | |
+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+
| | | | | | Elicitation Execution | | | |
+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+---------------+
| | | | | | | | | Implementation |
+===============+===============+===============+===============+===============+===============+===============+===============+===============+===============+===============+===============+

## 3.4 Functional Requirements

### 3.4.1 Dissatisfier Requirements

#### 3.4.1.1 Requirement 1

---

**Requirements:** User Authentication and Authorization

---

**Description:** The system shall provide a secure login mechanism
for students, lecturers, parents, and admins

**Elicitation Interview with lecturers, survey conducted towards
Activities:** parents and students

**Responsible Iman Nadhirah Binti Mohd Hafiz
Member:**

**Supporting Question 1 ([[Interview
Documents:** 1]{.underline}](#interview-1)), Question1
([[Interview 2]{.underline}](#interview-2)),
Question 9 ([[Parents
survey]{.underline}](#parents)), Question 13
([[Student survey]{.underline}](#students))

**Related Login
Function:**

---

#### 3.4.1.2 Requirement 2

---

**Requirements:** View Academic Grades

---

**Description:** The system shall allow users (students,lecturers,
parents) to view academic grades securely

**Elicitation Interview with lecturers, survey conducted towards
Activities:** parents and student

**Responsible Phartiban A/L Kumarhesan
Member:**

**Supporting Question 2 and 10 ([[Interview
Documents:** 1]{.underline}](#interview-1)), ([[Interview
2]{.underline}](#interview-2)), Question 1
([[Parent Survey]{.underline}](#parents))

**Related View academic grades
Function:**

---

#### 3.4.1.3 Requirement 3

---

**Requirements:** Access Attendance Records

---

**Description:** The system shall allow students, parents, and
lecturers to access and monitor attendance records.

**Elicitation Interview with lecturers, survey conducted towards
Activities:** parents

**Responsible Suzannah Pancer
Member:**

**Supporting Question 4&5 ([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2)), Question 2&3
([[Parent Survey]{.underline}](#parents))

**Related Check class attendance records
Function:**

---

#### 3.4.1.4 Requirement 4

---

**Requirements:** Access Academic Timetable

---

**Description:** The system shall display each user's course
schedule or timetable.

**Elicitation Interview with lecturers, Questionnaire with
Activities:** parents

**Responsible Nurul Natasha Adilyn Binti Fadzil
Member:**

**Supporting Question 8 ([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2)), Question7 ([[Parent
Survey]{.underline}](#parents))

**Related Access and view course schedule/timetable
Function:**

---

#### 3.4.1.5 Requirement 5

---

**Requirements:** Manage User Accounts and Roles

---

**Description:** The system shall enable admin to assign roles and
manage user account permissions.

**Elicitation Interview with Admin
Activities:**

**Responsible Iman Nadhirah Binti Mohd Hafiz
Member:**

**Supporting Question 1&8 ([[interview
Documents:** 3]{.underline}](#interview-3))

**Related Manage user accounts and system configurations
Function:**

---

#### 3.4.1.6 Requirement 6

---

**Requirements:** Integration with Campus Systems

---

**Description:** The system shall integrate with CMS, LMS, and
calendar systems to sync data.

**Elicitation Interview with Admin
Activities:**

**Responsible Phartiban A/L Kumarhesan
Member:**

**Supporting Question 2 ([[interview
Documents:** 3]{.underline}](#interview-3))

**Related Integrate and Sync with CMS, LMS, and calendar
Function:** systems

---

#### 3.4.1.7 Requirement 7

---

**Requirements:** Maintain Data Privacy and Access Permissions

---

**Description:** The system must enforce data security and
appropriate access levels.

**Elicitation Interview with Admin
Activities:**

**Responsible Suzannah Pancer
Member:**

**Supporting Question 8 ([[interview
Documents:** 3]{.underline}](#interview-3))

**Related Maintain data privacy and access permissions
Function:**

---

#### 3.4.1.8 Requirement 8

---

**Requirements:** Pay Tuition and Other Fees

---

**Description:** Ability to make fee payments through the portal

**Elicitation Observation
Activities:**

**Responsible Phartiban A/L Kumarhesan
Member:**

**Supporting Question 5 ([[interview
Documents:** 3]{.underline}](#interview-3))

**Related Pay tuition and other fees
Function:**

---

#### 3.4.1.9 Requirement 9

---

**Requirements:** View Payment History and Invoices

---

**Description:** View historical tuition and fee records

**Elicitation Observation
Activities:**

**Responsible Phartiban A/L Kumarhesan
Member:**

**Supporting Question 5 ([[interview
Documents:** 3]{.underline}](#interview-3))

**Related View Payment History and Invoices
Function:**

---

###

###

### 3.4.2 Satisfier Requirements

#### 3.4.2.1 Requirement 10

---

**Requirements:** Upload and Manage Grades

---

**Description:** Lecturers shall be able to upload, confirm, and
manage student grades.

**Elicitation Interview with Lecturers
Activities:**

**Responsible Nurul Natasha Adilyn Binti Fadzil
Member:**

**Supporting Question 2&3([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2))

**Related Upload student grades
Function:**

---

#### 3.4.2.2 Requirement 11

---

**Requirements:** Digital Attendance Tracking

---

**Description:** The system shall support digital attendance marking
and tracking over time.

**Elicitation Interview with Lecturers
Activities:**

**Responsible Iman Nadhirah Binti Mohd Hafiz
Member:**

**Supporting Question 4&5 ([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2))

**Related Mark and manage attendance records
Function:**

---

#### 3.4.2.3 Requirement 12

---

**Requirements:** Post Announcements and Updates

---

**Description:** Lecturers and admins shall post class and global
announcements

**Elicitation Interview with Lecturers
Activities:**

**Responsible Phartiban A/L Kumarhesan
Member:**

**Supporting Question 6&7 ([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2))

**Related Post class announcements and updates
Function:**

---

####

#### 3.4.2.4 Requirement 13

---

**Requirements:** Dashboard with Performance Overview

---

**Description:** The system shall provide academic dashboard with
grade and attendance insights.

**Elicitation Interview with Lecturers
Activities:**

**Responsible Suzannah Pancer
Member:**

**Supporting Question 10([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2))

**Related Monitor student academic performance
Function:**

---

#### 3.4.2.5 Requirement 14

---

**Requirements:** Submit Feedback and Support Requests

---

**Description:** The system shall allow users to submit feedback and
helpdesk tickets.

**Elicitation Interview with Admin and survey conducted towards
Activities:** students

**Responsible Nurul Natasha Adilyn Binti Fadzil
Member:**

**Supporting Question 6 ([[interview
Documents:** 3]{.underline}](#interview-3)), Question 18
([[Student survey]{.underline}](#students))

**Related Submit Feedback/Support Tickets, Submit Helpdesk
Function:** Tickets

---

#### 3.4.2.6 Requirement 15

---

**Requirements:** Alert and Reminder System

---

**Description:** The system shall send deadline reminders and
important alerts to users.

**Elicitation Interview with Lecturer and survey towards students
Activities:**

**Responsible Iman Nadhirah Binti Mohd Hafiz
Member:**

**Supporting Question 9([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2)), Questionnaire Q3,
Q4, Q12

**Related Receive SMS/Email alerts
Function:**

---

###

### 3.4.3 Delighter Requirements

#### 3.4.3.1 Requirement 16

---

**Requirements:** Notification Read Tracking

---

**Description:** The system may notify lecturers or admins when
users view or interact with announcements.

**Elicitation Interview with lecturers
Activities:**

**Responsible Phartiban A/L Kumarhesan
Member:**

**Supporting Question 7([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2))

**Related View announcements and academic notifications
Function:**

---

#### 3.4.3.2 Requirement 17

---

**Requirements:** Custom Notification Preferences

---

**Description:** Parents may configure notification delivery method
(SMS, email, or both).

**Elicitation Survey towards parents
Activities:**

**Responsible Suzannah Pancer
Member:**

**Supporting Question 14 ([[Parent
Documents:** Survey]{.underline}](#parents))

**Related Receive SMS/Email alerts
Function:**

---

#### 3.4.3.3 Requirement 18

---

**Requirements:** Visual Performance Analytics

---

**Description:** The system may display graphs and visual trends of
student performance over time.

**Elicitation Interview with lecturer
Activities:**

**Responsible Nurul Natasha Adilyn Binti Fadzil
Member:**

**Supporting Question 10 ([[Interview
Documents:** 1]{.underline}](#interview-1)),([[Interview
2]{.underline}](#interview-2))

**Related Monitor student academic performance
Function:**

---

#### 3.4.3.4 Requirement 19

---

**Requirements:** Mobile-Friendly Responsive Interface

---

**Description:** The portal may be optimized for mobile devices
across Android and iPhone.

**Elicitation Interview with admin and survey towards students
Activities:**

**Responsible Iman Nadhirah Binti Mohd Hafiz
Member:**

**Supporting Question 5 ([[interview
Documents:** 3]{.underline}](#interview-3)), Question
7&12([[Student survey]{.underline}](#students))

**Related All access-related functions (Login, View Grades,
Function:** etc.)

---

## 3.5 Performance requirements

The performance requirements for the University Communication Service
Portal are specified below. These requirements include both static and
dynamic numerical requirements, ensuring the system meets necessary
performance standards for usability and efficiency.

### 3.5.1 Static Numerical Requirements

1.  **Storage Scalability**

- The system shall support a minimum of 2 TB of storage capacity for
  academic records, attendance logs, user data and media uploads.
  However data storage usage does not exceed the maximum during peak
  periods for load controls.

- The portal shall perform database backups every 12 hours to prevent
  data lost in the system. Back ups are stored securely and restorable
  within 30 mins of request.

- The system shall retrieve students records, attendance and schedules
  within ≤ 2 seconds of request submission

2.  **Simultaneous user capacity**

- The system shall accommodate up to 5,000 current users during peak
  usage periods. The system shall remain stable without crashes or
  latency over 2 seconds for most of user actions.

- The system shall automatically timeout a user session after 15 minutes
  of inactivity. Inactive sessions are logged out securely with session
  data cleared all the time.

###

### 3.5.2 Dynamic Numerical Requirements

1.  **Task handling**

- The system shall maintain a 99.5% task completion success rate for
  automated operations such as notifications handout, QR code
  generation, and schedule exports. With automated logs showing less
  than 0.5% failure rate in task processing.

- The system shall maintain an uptime of 99.9% on a monthly basis,
  accounting for maintenance windows which is a critical criteria for
  every system

- The system shall maintain a 95% responsiveness rate across all core
  features in the portal such as in dashboard, notifications, and user
  profile update. User interaction logs will confirm the stable
  performance.

- During concurrent usage of more than 4,000 users, the system shall
  maintain a task success rate of above 95% across all modules.

2.  **Data Processing**

- The system shall ensure that more than 98% of background data
  synchronization tasks with University Management System and Campus
  Management System are completed within 5 seconds of interaction. Audit
  logs will show timely and accurate data reflection.

<!-- -->

- The system shall ensure that more than 97% of submitted grade uploads
  are processed without manual intervention or error correction.

<!-- -->

- The system shall deliver more than 95% of generated reports on grades
  or attendance to the user within 10 seconds under normal load.

3.  **Peak Load Conditions**

- Under peak load conditions the system shall process at least 90% of
  user requests within 5 seconds. Stress testing results must be less
  than 10% for slow or failed requests.

4.  **Transaction handling**

- The system shall successfully process more than 95% of all
  transactions including login, course registration and grade
  submissions within 2 seconds under normal operating conditions. The
  transaction logs will show 95% of actions completed under 2 seconds.

These performance requirements ensure that the system will be responsive
and efficient, providing a seamless experience for students, parents,
and lecturers even under heavy usage conditions. Each requirement is
stated in measurable terms to facilitate testing and validation.

## 3.6 Usability Requirements

The usability and quality in user requirements for the University
Communication Service Portal system aims to ensure that the software is
efficient, satisfying and productive for the intended users. These
requirements encompass measurable criteria for effectiveness, efficiency
and satisfaction and the prevention of future issues that could arise
from its user specific contexts.

### 3.6.1 User Interface

1.  Consistent Layout and Design

- The system shall provide a consistent and intuitive user interface
  across all modules to support users with varying levels of technical
  expertise, especially first year students and parents with limited
  digital literacy.

2.  Responsive Design

- The system shall support responsive web design, ensuring usability
  across desktop, tablet and mobile devices without requiring separate
  portals.

### 3.6.2 User Experience

1.  Efficient Navigation

- The system shall provide intuitive navigation pathways through the
  portal, to enable quick and smooth allocation of information and
  functionalities navigation.

- The system shall minimize the number of steps required to reach an
  intended function like viewing grades, checking attendance and
  registering courses.

2.  Personalized Recommendations

- The system shall adhere to Web Content Accessibility Guidelines (WCAG
  2.1 Level AA) to ensure usability for users with impaired
  disabilities, including screen reader compatibility, keyboard
  navigation and appropriate colour contrast.

### 3.6.3 Communication

1.  Feedback Mechanism

- The system shall offer real time feedback after user's actions such as
  form submission, file uploads or registration to enhance user
  confidence and clarity.

2.  Language Standards

- The system shall use clear, non-technical language in all on-screen
  instructions, alerts and error messages to accommodate users with
  diverse educational backgrounds.

3.  Notification Managements

- The system shall allow users to customize notification preferences,
  including SMS alerts and email notifications, to improve
  communications effectiveness and user satisfaction.

### 3.6.4 Data protection

1.  Data Encryption

- The system shall automatically log out users after a period of
  inactivity to prevent unauthorized access to sensitive data and
  protect users sessions.

2.  Server controls

- The system shall use encrypted channels (HTTPS) for all communication
  between clients and server, ensuring data transmission is secure from
  interception.

##

##

## 3.7 Logical Database Requirements

The logical requirements section defines the essential components and
operations of an integrated platform designed to support academic
communication and services for students, parents, lecturers, and
administrators. It outlines the types of academic and administrative
data accessed by each user group, the frequency of operations such as
grade uploads, attendance monitoring, and course registration, and
access privileges based on user roles. It also includes integrity
constraints to maintain consistent academic records, security protocols
such as authentication and role-based access control, and data retention
requirements to preserve historical academic and financial data in
compliance with institutional policies.

### 3.7.1 Class Diagram

The following figure shows the class diagram of EduAxis.

![](media/image2.png){width="6.0167782152230975in"
height="6.077451881014873in"}

_Figure 3.8.1 Class Diagram_

### 3.7.2 Data Entities

The following table describes the key data entities and their
functionalities in the University Portal System.

_Table 3.8.2.1 Data Entities and Descriptions_

---

**Data Entity** **Description**

---

User An abstract class representing all
users (Student, Parent, Lecturer,
Admin). Each user can register, log
in, and access role-based features.

Student A subclass of User with attributes
such as studentID, name, program,
year, and parentID. Students can
view grades, attendance, and make
payments.

Parent A subclass of User with parentID
and linked student accounts.
Parents can monitor academic
records and tuition status of their
children.

Lecturer A subclass of User with attributes
such as lecturerID, department, and
courseList. Lecturers can manage
grades, attendance, and
announcements.

Admin A class representing the system
administrator, responsible for user
management, system configuration,
and integration of third-party
tools.

Course A class representing academic
courses offered by the institution.
Attributes include courseID,
courseName, creditHours, semester,
and lecturerID.

Registration An association class linking
Students and Courses for each
semester. Attributes include
registrationID, studentID,
courseID, and semester.

Grade A class storing student grades for
courses. Attributes include
gradeID, studentID, courseID, and
gradeValue.

Attendance A class tracking student
attendance. Attributes include
attendanceID, studentID, courseID,
date, and status.

Payment A class recording tuition and other
fee transactions. Attributes
include paymentID, studentID,
amount, dueDate, datePaid, and
status.

Message A class for internal messaging
among users. Attributes include
messageID, senderID, receiverID,
content, and timestamp.

Announcement A class for official notifications
from lecturers or admins. Includes
announcementID, title, content,
createdBy, targetGroup, and
timestamp.

FeedbackTicket A class representing user-submitted
feedback or issues. Attributes
include ticketID, userID,
description, status, and
createdDate.

---

### 3.7.3 Relationship

The following table describes the relationships between each class in
the EduAxis system.

_Table 3.8.3.1 Relationships between Classes_

---

**Entity** **Description**

---

User This abstract class is inherited by Student, Parent,
Lecturer, and Admin. Each user can log in and access
features according to their role.

Student Students can register for courses, view grades and
attendance, submit feedback, make payments, and
receive messages. Each student is linked to one or
more parents.

Parent Parents monitor academic records and payment status
for one or more children (students). Each parent is
associated with one user account.

Lecturer Lecturers manage attendance, upload grades, post
announcements, and oversee courses they teach. A
lecturer is associated with one user account and
multiple courses.

Admin Admins manage system configurations, users,
integrations, announcements, and helpdesk support.
Each admin is a standalone user.

Course Courses are managed by lecturers and linked to
students through the Registration entity. Each
course is taught by one lecturer and can have many
students.

Registration Associates students with courses for a specific
semester. A student can register for multiple
courses and a course can have many students.

Grade Grades are recorded for students per course. Each
grade entry is linked to one student and one course.

Attendance Attendance records are associated with a specific
student and course on a given date. One student has
many attendance entries.

Payment Payment records are created per student. Each
student can have multiple payments linked to
invoices and fee types.

Message Internal messages are exchanged between users. A
user can send and receive many messages.

Announcement Announcements are created by lecturers or admins and
targeted to specific user groups such as students or
parents. Each user can view multiple announcements.

FeedbackTicket Feedback or complaints are submitted by users. Each
ticket is linked to one user and may be addressed by
admin.

---

### 3.7.4 Types of Information Used by Various Functions

_Table 3.8.4.1 Types of Information, Classes Involved, and Functions_

---

**Type** **Classes Involved** **Functions**

---

User Information User, Student, Parent, Login, authentication, profile
Lecturer, Admin management, permission assignment

Academic Record Grade, Course, Attendance Viewing academic performance,
Information calculating GPA, managing class
records

Course Registration, Course Registering/dropping courses,
Registration assigning lecturers, timetable
Information generation

Financial Payment, Invoice Fee payment tracking, generating
Information payment history, triggering payment
reminders

Communication Message, Announcement Internal messaging, posting
Information system-wide or class-specific
announcements

Support & FeedbackTicket Submitting, tracking, and
Feedback responding to
student/parent/lecturer feedback

Notification Notification, Configuring and triggering
Preferences NotificationPreferences SMS/Email alerts

Integration ExternalSystem Syncing with CMS, LMS, Auth
Information service, SMS gateway, and payment
APIs

---

### 3.7.5 Frequency of Use

_Table 3.8.5 Frequency of Operation Usage and Description_

---

**Operation** **Frequency** **Description**

---

User Authentication High Includes user login and
logout for students,
parents, lecturers and
administrators. Access
personalized portal
features securely.

Academic Data Medium Includes entering,
Management updating and retrieving
grades, reports and
academic progress by
lecturers and students.

Attendance Processing High QR code generation,
student check-in,
attendance validation
and database updates.

Course Management Low Encompasses course
registration, schedule
view and updates,
course swap or drop by
students and lecturers

Financial Records Medium Involves fee billing,
Handling payments confirmation,
balance checking by
students and parents.

Communication and High Includes SMS alerts,
Notifications email notifications,
and portal
announcements related
to attendance, grades
and fees.

Data Report and Export Medium Includes generation and
download of grade
lists, attendance
summaries and
performance reports in
PDF/CSV format.

Resource Access Medium Includes accessing
integrated systems such
as LMS, library
resources and academic
support services from
the portal.

---

###

### 3.7.6 Accessing Capabilities

_Table 3.8.6 Users Roles and Accessing Capabilities in the System_

---

**Role** **Capabilities**

---

Students Access and manage academic records, course
registration, fee payment, attendance and receive
timely notifications.

Parents Monitor a child\'s academic performance, financial
status, and receive alerts via SMS for better
engagements.

Lecturers Manage course related activities including uploading
academic grades, recording attendance, sharing
announcements and generating academic reports.

Administrators Full control over user management, system
configuration, academic scheduling, communication
settings and data reporting across the portal

---

###

### 3.7.7 Integrity Constraints

1.  **User Role Validation:**

> Each user must have one of the following roles: Student, Lecturer,
> Parents, Admin. This role must be validated upon user registration and
> updated if necessary.

2.  \*\*Unique Identifiers:\*\*
    All primary entities in the system including users, courses, grades,
    attendance records, and transactions must have unique identifiers
    (ID) to ensure accurate tracking and data retrieval

3.  **Foreign Keys:**

> Foreign key constraints must be enforced to maintain relationships
> between entities.

### 3.7.8 Security

1.  **Authentication and Authorization:**

> All users must log in using secure credentials. Access to system
> features will be managed using Role-Based Access Control (RBAC) to
> ensure users can only perform actions permitted by their role.

2.  **Data Encryption:**\
    Sensitive data such as passwords and authentication tokens must be
    encrypted using industry-standard encryption algorithms to ensure
    confidentiality and prevent unauthorized access.

3.  **Audit Trails:**

> The system must maintain logs for key activities such as grade
> submissions, attendance updates, profile changes, and payment
> transactions. Each log must include a timestamp, the user ID, and a
> description of the action performed.

###

### 3.7.9 Data Retention Requirements

1.  \*\*User Data\*\*
    Retained for the duration of system use and up to 2 years after
    account deactivation, or longer if legally required.

2.  \*\*Academic Records (Grades, Attendance, Schedule)\*\*
    Retained permanently for accreditation, transcript generation, and
    historical reference.

3.  \*\*Alert and Notification Logs\*\*
    Stored for up to 12 months for system audit and tracking purposes.

4.  \*\*Payment Records\*\*
    Retained for at least 7 years in compliance with university finance
    policies and national tax regulations.

##

## 3.9 Design Constraints

### 3.9.1 Compliance with Data Privacy Regulations

---

**Constraint The system must comply with relevant Malaysian data
Description** protection laws such as the Personal Data Protection Act
(PDPA), ensuring the security and confidentiality of all
student, parent, and staff data.

---

**Source** External regulatory requirements.

**Impact** All data collection, storage, and processing activities
must enforce consent policies, encrypted data
transmission, anonymization practices (where applicable),
and role-based access to sensitive information.

---

### 3.9.2 Integration with Existing University Systems

---

**Constraint The platform must seamlessly integrate with the
Description** university's existing systems, including the Campus
Management System (CLiC), Learning Management System
(eBwise), authentication systems, and SMS/email gateways.

---

**Source** Project limitations.

**Impact** The system must support RESTful APIs and conform to the
schemas and endpoints defined by current university IT
systems, ensuring backward compatibility and minimal
disruption.

---

### 3.9.3 Security Standards

---

**Constraint The system must follow best-practice security protocols
Description** and adhere to OWASP guidelines to ensure secure data
transmission, access control, and input validation.

---

**Source** External standards.

**Impact** All modules must include secure authentication, password
hashing, input sanitization, session timeout, and audit
logging. Penetration testing and security reviews must be
conducted regularly.

---

### 3.9.4 Accessibility Requirements

---

**Constraint The platform must comply with WCAG 2.1 (Web Content
Description** Accessibility Guidelines) to ensure equal access to all
user groups, including users with disabilities.

---

**Source** External accessibility standards.

**Impact** Support for screen readers, keyboard-only navigation, and
high contrast themes must be integrated. Form fields and
interactive content must be labeled clearly for
accessibility tools.

---

### 3.9.5 API Usage Limitations

---

**Constraint The portal must respect usage limitations for third-party
Description** APIs (e.g., Twilio SMS Gateway, LMS/CMS APIs), including
rate limits and authentication policies.

---

**Source** External API standards.

**Impact** The system must implement throttling, retry mechanisms,
and error handling routines to avoid service disruptions
when API limits are exceeded.

---

### 3.9.6 Performance and Scalability

---

**Constraint The portal must scale to support large user loads,
Description** particularly during critical periods such as registration,
grade release, or announcement events.

---

**Source** Project limitations.

**Impact** Use of load balancing, caching strategies, database
indexing, and asynchronous operations is required to
maintain system responsiveness.

---

### 3.9.7 User Experience Consistency

---

**Constraint The system must provide a consistent and intuitive
Description** experience across mobile and desktop devices.

---

**Source** Project limitations.

**Impact** Interfaces must be responsive and user-friendly,
minimizing clicks and displaying contextually relevant
information based on user roles (student, parent,
lecturer, admin).

---

### 3.9.8 Data Interoperability

---

**Constraint The system must support data exchange between different
Description** systems via standard formats such as JSON.

---

**Source** External standards.

**Impact** All integrations must use RESTful APIs with defined
input/output schemas to ensure smooth data flow with
minimal transformation overhead.

---

### 3.9.9 Legal and Ethical Considerations

---

**Constraint The system must protect user rights concerning the use,
Description** access, and visibility of their data, especially in
educational and financial contexts.

---

**Source** External legal requirements and ethical principles.

**Impact** Consent mechanisms must be enforced. Users should be able
to view what data is stored about them and request updates
or removals in accordance with policy.

---

### 3.9.10 Project Budget and Timeline

---

**Constraint The project must remain within the allocated budget and
Description** development timeline set by the university or academic
committee.

---

**Source** Project limitations.

**Impact** Design decisions must consider trade-offs between feature
richness and cost-efficiency. MVP-level features must be
prioritized to meet deadlines.

---

### 3.9.11 Standards Compliance

#### 3.9.11.1 Report Format

Requirements:

- Reports involving personal or academic data must be exported in PDF
  format.

- Reports must include system logs, student performance summaries, fee
  transactions, and attendance reports.

- Exported documents must maintain secure formatting, showing access
  dates, editors, and audit trails.

#### 3.9.11.2 Data Naming

Requirements:

- Personal data fields must follow clear naming conventions (e.g.,
  student_id, first_name, phone_number).

- Sensitive fields such as passwords must be encrypted and labeled
  (e.g., hashed_password, jwt_token).

- API endpoints must be REST-compliant and named semantically (e.g.,
  /api/v1/students/:id/courses, /api/v1/payments/:id).

#### 3.9.11.3 Accounting Procedures

Requirements:

- Data access logs must capture who accessed what, when, and what action
  was performed.

- Audits must be scheduled quarterly, covering access control, backup
  recovery, and data leaks.

- API usage statistics and failure rates must be recorded.

- Financial records and invoice statuses must be traceable to user ID
  and timestamp.

#### 3.9.11.4 Audit Tracing

Requirements:

- All sensitive changes (profile updates, password resets, permission
  changes) must be logged.

- Transactions and ticket actions must be time stamped with admin/actor
  details.

- Failed login attempts and suspicious API activity must trigger system
  alerts.

- Changes to access rules, course records, or student academic data must
  include before/after values.

**All standards and practices referenced are aligned with: PDPA
(Malaysia), OWASP, WCAG 2.1, RESTful API (RFC 7231), and internal
academic IT policies.**

## 3.10. Software system attributes

### 3.10.1 Reliability

**3.10.1.1. System Uptime**

The University Communication and Services Portal shall maintain an
uptime of 99.9%, ensuring continuous availability for students,
lecturers, parents, and administrators.

**3.10.1.2. Data Integrity**

The system shall maintain data integrity by enforcing **transactional
controls** and validation checks. All data updates shall follow **ACID**
principles to prevent data corruption.

**3.10.1.3. Backup and Recovery**

The system shall perform automated daily backups of essential data,
including user profiles, academic records, and payment transactions.
Backup data shall be stored securely, with automated recovery procedures
in place for system failures.

### 3.10.2 Availability

**3.10.2.1 Redundancy**

The system shall utilize redundant servers and failover mechanisms to
maintain service availability during hardware failures or maintenance
periods.

**3.10.2.2. Maintenance Windows**

Scheduled maintenance windows shall be communicated to users at least 48
hours in advance, and maintenance activities shall be planned during
off-peak hours to minimize disruption.

**3.10.2.3. Real Time monitoring**

The system shall implement real-time monitoring tools to track system
performance and availability, allowing for immediate detection and
response to any issues that arise.

###

### 3.10.3 Security

**3.10.3.1. Cryptographic Techniques**

The system shall utilize industry-standard cryptographic techniques to
protect sensitive data. All user passwords shall be hashed using a
strong hashing algorithm, and all sensitive data transmissions shall be
encrypted using TLS (Transport Layer Security).

**3.10.3.2. Logging and Monitoring**

The system shall maintain detailed logs of all user activities and
system events. These logs shall be stored securely and monitored
regularly to detect and respond to suspicious activities.

**3.10.3.3. Module Separation**

Authentication, academic processing, and financial modules shall be
**logically separated** to reduce the risk of unauthorized access or
data leakage.

**3.10.3.4. Communication Restrictions**

Access between modules shall be restricted based on the principle of
least privilege, ensuring only authorized components interact with
sensitive services.

**3.10.3.5. Data Integrity Checks**

Automated integrity checks shall verify the consistency of critical
records (e.g., grade reports, fee balances), with alerts for
unauthorized or inconsistent changes.

**3.10.3.6. Data Privacy Assurance**

The system shall implement privacy controls, allowing users to manage
their data and preferences, and ensuring compliance with data protection
regulations.

###

### 3.10.4. Maintainability

**3.10.4.1. Modular Design**

The platform shall be developed using a modular architecture, allowing
components (e.g., grade module, attendance module) to be independently
updated or maintained.

**3.10.4.2. Documentation**

Comprehensive system documentation shall include code-level comments,
API references, user manuals, and deployment guides to support future
development and maintenance.

**3.10.4.3. Bug Tracking and Resolution**

A bug tracking system shall be implemented to log, prioritize, and
resolve issues, with classification by severity and assigned response
times.

### 3.10.5. Portability

\*\*3.10.5.1. Platform Independence\*\*
The system shall be designed to be platform-independent, supporting
deployment on Windows, Linux, or macOS environments without major
rework.

\*\*3.10.5.2. Containerization\*\*
The system shall support Docker-based containerization, ensuring
consistent deployment across development, staging, and production
environments.

\*\*3.10.5.3. External Libraries and Dependencies\*\*
Dependencies on platform-specific tools shall be minimized.
Cross-platform libraries shall be prioritized to improve portability and
long-term support.

##

# Supporting information

## 4.1 Interview

The purpose of these interview sessions is to elicit requirements and
insights for the University Communication and Service Portal from
students, parents, lecturers and administrators of the system itself.
The focus of this interview is to obtain opinion on the portal's
functions, features and design for improvements and developments.

### 4.1.1 Interview 1

#### 4.1.1.1 Interview Preparation

+-------------------+-----------------------------------------------------+
| **Stakeholder | Mr. Deepak Kumar Lecturers of Multimedia University |
| Details:** | |
+-------------------+-----------------------------------------------------+
| **Date and | 15/5/2025 |
| Time:** | |
+-------------------+-----------------------------------------------------+
| **Interviewers:** | Suzannah Pancer |
| +-----------------------------------------------------+
| | Iman Nadhirah Binti Modh Hafiz |
+===================+=====================================================+

#### 4.1.1.2 Interview Agenda

---

No. Question Response

---

1\. How important is it Quick and secure login is important to ensure
for you to log in smooth access to teaching tools and student
quickly and securely data, which supports efficiency in handling
to access the daily academic tasks.
academic portal?

2\. What challenges do Although I prefer manual methods, an
you currently face efficient grade upload feature would reduce
when uploading manual effort, improve consistency, and
student grades, and simplify the grading process, especially when
how would a grade handling large numbers of students.
upload feature help  
 you?

3\. How would you feel A system that automatically confirms and
about a system that saves grades would be helpful in minimizing
confirms and saves errors and ensuring that no data is lost
each grade you upload during entry, which adds reliability to the
automatically? grading process.

4\. How do you currently Attendance is currently taken manually during
mark attendance, and class, with flexibility for absences based on
would a digital valid student explanations. I acknowledge
attendance tracker that a digital attendance tracker would
improve your improve efficiency, even though they still
efficiency? prefer manual observation for personal
engagement.

5\. Would it be helpful Yes, the ability to view, edit, and track
if the system allowed attendance records digitally would support
you to view, edit, better monitoring and make it easier to
and monitor manage exceptions or identify patterns in
attendance records student attendance.
over time?

6\. How useful would it A centralized platform for announcements
be to post would be useful to ensure that all students
announcements or receive updates consistently and in a timely
class updates in one manner, supporting better communication.
place where all  
 students can see  
 them?

7\. Do you think Yes, receiving such notifications would be
receiving a beneficial for tracking student
notification when responsiveness and ensuring that important
students view or information is being read and acknowledged.
respond to  
 announcements would  
 be beneficial?

8\. How often do you Integration of the academic calendar into the
refer to the academic dashboard would be valuable for keeping track
calendar, and how of schedules and aligning class activities
important is it for with institutional deadlines.
you to have it  
 integrated into your  
 dashboard?

9\. Would you find it Yes, alerts for upcoming deadlines would be
valuable if the very helpful in managing time-sensitive
system alerted you academic tasks and avoiding last-minute
about upcoming pressure.
deadlines, like grade
submissions or exam  
 dates?

10\. How helpful would it This feature would definitely be helpful.
be if the system While I rely heavily on personal observation
could show an and judgment in class, having a centralized
overview of each performance overview would support better
student's tracking and offer additional insight into
performance, student progress.
including grades and  
 attendance?

---

#### 4.1.1.3 Proof

![](media/image3.png){width="4.041666666666667in"
height="3.18792104111986in"}

Figure 4.1.1.3.1- Interview with Mr Deepak Kumar, FCI Lecturer Of
Multimedia University Cyberjaya

The Lecturer provides valuable feedback throughout the interview on
functions and features of the portal usability and preferences. Lecturer
inputs have been incorporated into the functional requirements to ensure
practical and academic relevance.

### 4.1.2 Interview 2

#### 4.1.2.1 Interview Preparation

+-------------------+-----------------------------------------------------+
| **Stakeholder | Dr. Kairulanuar Bin Ab kadir Lecturers of |
| Details:** | Multimedia University |
+-------------------+-----------------------------------------------------+
| **Date and | 15/5/2025 |
| Time:** | |
+-------------------+-----------------------------------------------------+
| **Interviewers:** | Suzannah Pancer |
| +-----------------------------------------------------+
| | Iman Nadhirah Binti Modh Hafiz |
+===================+=====================================================+

#### 4.1.1.2 Interview Agenda

---

No. Question Response

---

1\. How important is it Quick and secure login is important for
for you to log in accessing the system efficiently, especially
quickly and securely when managing large numbers of students and
to access the time-sensitive tasks like grade submissions
academic portal? and attendance tracking.

2\. What challenges do I face significant challenges due to the
you currently face large volume of students (sometimes
when uploading 800--1000) and numerous assessments such as
student grades, and quizzes, tests, and projects. It becomes
how would a grade time-consuming and tedious to upload multiple
upload feature help components manually. There's also difficulty
you? in ensuring consistency across different
lecturers, with no automated alerts if
discrepancies arise in grading. A
well-designed grade upload feature could
streamline the process, offer validation or
alerts for inconsistencies, and reduce errors
before final submission to the examination
unit.

3\. How would you feel This would be highly beneficial. Having a
about a system that confirmation system that flags potential
confirms and saves issues before submission---especially when
each grade you upload working with other lecturers---would reduce
automatically? human errors and prevent issues during the
review by the examination unit.

4\. How do you currently Previously, attendance was taken manually
mark attendance, and (calling names), and later using QR codes.
would a digital The lecturer agrees that a digital tracker
attendance tracker would improve efficiency, especially since
improve your MMU is already working with system developers
efficiency? to enhance the credit-based system. Digital
tracking would also make the process faster
and more organized.

5\. Would it be helpful Yes, having a history of attendance records
if the system allowed would be helpful to evaluate patterns or
you to view, edit, identify students with poor attendance. It
and monitor would also support more data-driven
attendance records interventions if integrated properly.
over time?

6\. How useful would it Centralized announcement posting is implied
be to post to be useful as I discussed integrating
announcements or multiple student engagement and communication
class updates in one functions within the portal.
place where all  
 students can see  
 them?

7\. Do you think Usually I monitor student engagement through
receiving a the system. Therefore, having such a feature
notification when would be considered useful for tracking
students view or responsiveness and encouraging accountability
respond to among students.
announcements would  
 be beneficial?

8\. How often do you Time pressure was mentioned as a key
refer to the academic challenge---especially during grading
calendar, and how periods---so having academic deadlines and
important is it for the calendar integrated into the dashboard
you to have it would help in better planning and time
integrated into your management.
dashboard?

9\. Would you find it Absolutely. A I have mentioned the tight
valuable if the timeframes for marking exams, especially when
system alerted you exam schedules fall near the end of the
about upcoming semester. System alerts would help ensure
deadlines, like grade that deadlines are met without last-minute
submissions or exam stress.
dates?

10\. How helpful would it Very helpful. I strongly support this idea,
be if the system suggesting features like visual progress
could show an tracking (e.g., graphs over semesters),
overview of each predictive analytics, and data-driven
student's feedback. They also proposed using such data
performance, for early intervention or even AI-based
including grades and predictions of future performance. This level
attendance? of detail would allow lecturers to analyze
trends and offer more tailored academic
support.

---

#### 4.1.2.3 Proof

![](media/image4.png){width="5.994995625546807in"
height="3.378998250218723in"}

Figure 4.1..3.1- Interview with Dr Kairulanuar , FCI Lecturer Of
Multimedia University Cyberjaya

The Lecturer provides valuable feedback throughout the interview on the
importance of data visibility, automation, and customization in
supporting lecturers\' teaching workflows. Their feedback will guide the
enhancement of the academic modules and ensure the University
Communication and Service Portal aligns with teaching needs across
faculties.

###

### 4.1.3 Interview 3

#### 4.1.3.1 Interview Preparation

---

**Stakeholder Mr. Zaki Syahmi Bin Zulkifli, Officer of Multimedia
Details:** University Student Lifestyle and Experience
Department

---

**Date and Time:** 15/5/2025

**Interviewers:** Phartiban , Natasha Adilyn

---

#### 4.1.3.2 Interview Agenda

---

No. Question Response

---

1\. How should user roles User roles should be provided based on
(student, lecturer, verified student and staff records in the
admin, parent) be CMS. Role creation should be automated
managed and through syncing with CMS where students,
provisioned in the lecturers, and parents are auto-assigned
system? their roles upon registration. On the other
part, admin roles should be manually assigned
with strict approval workflows.

2\. How should the Integrating with CLiC is really crucial for
University syncing data such as grades, attendance, and
Communication and fee records. For the LMS or eBwise in our
Service Portal case, it should pull the assignment statuses
integrate with and push grades. Also, SMS gateway should be
existing systems such connected to the portal to trigger alerts for
as the Campus low attendance, overdue payments and other
Management System announcements.
(CLiC), LMS, and SMS  
 gateway?

3\. How often should Backups should be performed daily for
backups be performed, critical databases like user data and
and where should they academic records. We are looking forward to
be stored? both on-site and cloud-based backups where a
copy of backup is stored on MMU's internal
backup server and is also pushed to secure
cloud location something like AWS S3 with
encryption.

4\. What are the most The most common issues reported by users are
common support mostly on attendance records and notification
requests or issues delivery problems. Occasionally, we get
reported by users parent inquiries about login issues or
recently? problems in fee info.

5\. Should the portal be It would be better if the portal is optimized
optimized for mobile for mobile use as the majority of students
use? If yes, what and lecturers use mobile phones to access
devices are most systems. Android smartphone devices are the
commonly used? most commonly used based on our findings,
followed by iPhones. The UI should be
responsive especially for functions like
viewing announcements, checking schedules,
submitting feedbacks and so on.

6\. Should students be Yes, sure. This feature is useful for both
able to submit students and admin side, which is us so that
complaints or the raised feedback or complaints can be
feedback through the routed to the relevant department or admin.
portal? This is important as we can improvise the
system in future which also involves the
benefit of transparency and faster issue
resolution.

7\. What specific In terms of specific information or tasks
information or tasks each user should be able to access or
should each user type perform, it might be that first of all, let's
(student, lecturer, go for the students\' side. Students should
parent, admin) be be able to view grades, attendance,
able to access or announcements, pay fees, submit coursework
perform? and feedback. On the other side, parents
should be given access to view a child\'s
grades and fee status, get alerts, and
optionally view timetables. Moving on to
lecturers, they should be able to upload
grades, mark attendance, post class updates,
manage assignments. Finally, admins should
have the access to manage accounts, handle
integrations, send announcements, control
permissions, and respond to helpdesk tickets.

8\. What level of user It should be role-based at a minimum, with
management and the ability to assign custom permissions for
permissions control sub-roles such as department-level admins.
is required? Certain functions like announcements or user
deletion should only be allowed by system
admins.

---

#### 4.1.3.3 Proof

![](media/image5.png){width="4.96004593175853in"
height="3.7421773840769905in"}

Figure 4.1.3.3.1- Interview with Mr. Zaki Syahmi Bin Zulkifli, Officer
of Multimedia University Student Lifestyle and Experience Department

The system Administrator provided critical insights into the technical
backbone and operational expectations of the portal. Their input will
shape the infrastructure design, security measures and integration
strategies to ensure system reliability and compliance.

## 4.2. Survey

### 4.2.1 Students

Question 1: How do you currently access the following information?

-Grades and Academic Performance

\- Attendance and Class Schedule

-Tuition Fee information and Payments

-Meeting or Consultation Hours

-Notifications or Announcements from Lecturers

![](media/image6.png){width="6.5in" height="2.3055555555555554in"}

Question 2: Are you satisfied with the current process for accessing
that information?

![](media/image7.png){width="5.885416666666667in"
height="1.7031364829396325in"}

Question 3:Which platform do you find most convenient for accessing
university services and information?

![](media/image8.png){width="6.194398512685915in"
height="1.6208136482939632in"}

Question 4: Which of the following features would you like to have in
the portal?

![](media/image9.png){width="6.369792213473316in"
height="1.6502055993000875in"}

Question 5: How important is it for the portal to have a User-Friendly
interface?

![](media/image10.png){width="6.61625in" height="1.9645516185476815in"}

Question 6: How important is it for the portal to have Data Accuracy

![](media/image33.png){width="6.511569335083115in"
height="1.6724923447069115in"}

Question 7:How important is it for the portal to be Mobile Friendly

![](media/image34.png){width="6.432292213473316in"
height="1.526687445319335in"}

Question 8: How important is it for the portal to have Fast Loading
Speed

![](media/image35.png){width="6.255208880139983in"
height="1.4908781714785653in"}

Question 9: How important is it for the portal to be integrated with the
Campus Management System

![](media/image36.png){width="6.281914916885389in"
height="1.5464818460192475in"}

Question 10: Would you prefer the portal to be available as:

![](media/image37.png){width="6.109375546806649in"
height="1.6994389763779527in"}

Question 11: How often do you experience difficulties in accessing
university- related information?

![](media/image38.png){width="6.453125546806649in"
height="1.5547681539807523in"}

Question 12: What device do you primarily use to access university
services?

![](media/image39.png){width="6.380208880139983in"
height="1.5102909011373578in"}

Question 13: Which method of authentication would you prefer for secure
access?

![](media/image40.png){width="6.453125546806649in"
height="1.538050087489064in"}

Question 14: How would you like to receive important university
notifications?

![](media/image41.png){width="6.526042213473316in"
height="1.697998687664042in"}

Question 15: What kind of alerts would you prefer to receive?

![](media/image42.png){width="6.484375546806649in"
height="1.6826541994750657in"}

Question 16: How frequently do you prefer to receive communication
updates?

![](media/image32.png){width="6.359375546806649in"
height="1.5332469378827647in"}

Question 17: In your experience, what gaps exist in the way university
information is shared with students?

![](media/image23.png){width="4.020833333333333in"
height="2.861111111111111in"}

Question 18:If you could add one feature to the University Communication
and Services Portal, what would it be and why?

![](media/image24.png){width="4.020833333333333in"
height="2.8194444444444446in"}

### 4.2.2 Parents

Question 1: How important is it for you to be able to view your child's
academic grades through the portal?

![](media/image25.png){width="5.234375546806649in"
height="1.6169006999125108in"}

Question 2: How important is it for you to be able to see your child's
attendance records?

![](media/image26.png){width="5.442708880139983in"
height="2.0154385389326333in"}

Question 3: How important is it for you to receive SMS alerts if your
child has low attendance?

![](media/image27.png){width="5.546875546806649in"
height="1.8537489063867016in"}

Question 4: [How important is it to receive SMS reminders when tuition
fees are due or unpaid?]{.mark}

![](media/image28.png){width="5.369792213473316in"
height="1.902214566929134in"}

Question 5: [How important is it to have a dashboard that shows your
child's academic performance clearly in one place?]{.mark}

![](media/image29.png){width="5.494792213473316in"
height="2.121046587926509in"}

Question 6: How important is it for you to receive notifications when
your child's grades are uploaded or updated?

![](media/image30.png){width="5.578125546806649in"
height="1.9219969378827646in"}

Question 7: How important is it for you to view your child's class
schedule or timetable through the portal?

![](media/image31.png){width="5.546875546806649in"
height="1.9960728346456693in"}

Question 8: [How important is it for the portal to also send updates and
alerts via email in addition to SMS?]{.mark}

![](media/image21.png){width="5.901753062117235in"
height="1.8954538495188102in"}

Question 9: [How important is it for the portal to have a secure and
private login for accessing your child's information?]{.mark}

![](media/image22.png){width="5.619792213473316in"
height="1.9924715660542431in"}

Question 10: [How important is it for the portal to work well on mobile
phones or tablets?]{.mark}

![](media/image51.png){width="5.692708880139983in"
height="2.1679483814523186in"}

Question 11: [How important is it for you to have access to payment
status and history for tuition and other fees?]{.mark}

![](media/image52.png){width="5.703125546806649in"
height="2.026819772528434in"}

Question 12: [How important is it to receive reminders about key
academic deadlines (e.g., registration, exam dates)?]{.mark}

![](media/image53.png){width="5.484375546806649in"
height="2.1704943132108485in"}

Question 13: [How important is it to receive alerts when your child
registers for or drops a course?]{.mark}

![](media/image54.png){width="5.526042213473316in"
height="1.9040507436570429in"}

Question 14: [How important is it to have the option to choose how you
receive alerts (SMS only, email only, or both)?]{.mark}

![](media/image55.png){width="5.755208880139983in"
height="2.0277416885389328in"}

##

##

##

## 4.3 Observation

### 4.3.1 CliC

url : [[https://clic.mmu.edu.my]{.underline}]{.mark}

Description: CLiC is a University Management Service Portal that serves
functions for users like students, lecturers and administrators or
Multimedia University (MMU) to manage and perform actions and get
records on academic and personal resources.

**4.3.1.1 Log In**

Description: allow users to log in with credentials given.

![](media/image56.png){width="6.302083333333333in"
height="3.4479166666666665in"}

_Figure 4.3.1.1 screenshot of CLiC login interface_

**4.3.1.2 Dashboard Features**

Description: All functions and features related to the user being logged
in will be provided in the dashboard. Students will be provided with
relevant functions such as personal information, campus finances,
attendance and academic records that are fully functional.

![](media/image57.png){width="6.5in" height="2.986111111111111in"}

_Figure 4.3.1.2 screenshot of CLiC Student Dashboard interface_

**4.3.1.3 Attendance records**

description : The attendance management allows students to keep track of
their class attendance progress throughout the trimester. This feature
also triggers students and parents\' email when a certain class
percentage drops below 80% that serves as an alert to the barring
process.

![](media/image58.png){width="6.5in" height="1.8333333333333333in"}

_Figure 4.3.1.3 screenshot of CLiC Student Attendance interface_

**4.3.1.4 Campus Finances**

description : The Campus Finances homepage provides a summary view of a
student's financial status at the university. It clearly displays the
total amount due, differentiating between \"Due Now\" and \"Future Due\"
payments. This centralized financial dashboard helps students manage
their tuition and other financial matters efficiently.

![](media/image48.png){width="6.5in" height="3.0416666666666665in"}

_Figure 4.3.1.4 screenshot of CLiC Student Campus finances interface_

**4.3.1.5 Class Schedule**

Description: The Class Schedule page interface provides students with a
clear, organized view of their academic timetable for the selected
trimester. This interface is designed to visually assist students in
tracking and managing their weekly class schedule with intuitive date
and time-based navigation.

![](media/image49.png){width="6.5in" height="2.888888888888889in"}

_Figure 4.3.1.5 screenshot of CLiC Student Class Schedule interface_

**4.3.1.6 Academic Records**

Description : The Academic Records Management interface provides
students with a centralized dashboard to access and manage essential
academic information throughout their studies. The other features
include a summary of academic progress, academic achievement and other
that is relevant to the student.

![](media/image50.png){width="6.5in" height="2.5694444444444446in"}

_Figure 4.3.1.6 screenshot of CLiC Student Academic Records interface_

### 4.3.2 eBwise

Url: https://ebwise.mmu.edu.my

**4.3.2.1 Login Page**

Description: Allows user to log in using SSO authentication.

![](media/image43.png){width="6.5in" height="3.3194444444444446in"}

_Figure 4.3.2.1 screenshot of eBwise Student login interface_

**4.3.2.2 Academic Managements Dashboard**

Description: The eBwise serves as a Communication Portal for both
student and lecturers to make and get updates on academic matters such
as announcements, assignments, and comments on class.

![](media/image44.png){width="6.5in" height="3.0833333333333335in"}

_Figure 4.3.2.2 screenshot of eBwise Student homepage interface_

**4.3.2.3 Announcement Page**

Description: The lecturer will be able to communicate and post
announcements to all or selected sections to notify students on
important updates.

![](media/image45.png){width="6.5in" height="3.0416666666666665in"}

_Figure 4.3.2.3 screenshot of eBwise Student announcements page
interface_

**4.3.2.4 Assignment Submission Managements**

Description: The lecturer assigns assignments with due date being set
and add submission button for file uploading purposes.

![](media/image46.png){width="6.5in" height="3.0555555555555554in"}

_Figure 4.3.2.4 screenshot of eBwise Student Assignment submission page
interface_

Description: The systems update submission status to the database and
notify lecturer on marking process.

![](media/image47.png){width="6.5in" height="3.0277777777777777in"}

_Figure 4.3.2.5 screenshot of eBwise Student Submitted Assignment follow
up page interface_

#

# 5. Verification

## 5.1. Verification of External Interfaces ([[3.2]{.underline}](#external-interfaces))

### 5.1.1 University Database Interface ([[3.2.1]{.underline}](#university-database-interface))

---

**Methods** Execute API calls to the PostgreSQL university
database and compare the response with expected
student, academic, and fee records. Scripts will be
used to test CRUD operations and role-based data
retrieval (such as student vs admin access).

---

**Responsibility** QA team and database administrators.

**Verification During integration testing and prior to each
time** deployment cycle.

**Environment** Development, staging, and production environments.

---

### 5.1.2 Campus Management System (CLiC) Interface ([[3.2.2]{.underline}](#campus-management-system-clic-interface))

---

**Methods** Perform API testing to verify grade, course
registration, and attendance data pulled from CLiC
matches internal student profiles. Use real
enrollment data and validate mapped fields.

---

**Responsibility** QA team and project integration lead.

**Verification During initial integration setup and after every
time** schema change or API update.

**Environment** Staging and production with controlled test users.

---

### 5.1.3 Learning Management System (eBwise) Interface ([[3.2.3]{.underline}](#learning-management-system-lms-interface))

---

**Methods** Verify grade upload and assignment sync via LMS API.
Compare LMS-side student submissions and scores
against portal display. Test API failures and
timeouts.

---

**Responsibility** QA team and LMS admin.

**Verification During LMS sync cycles and before academic term
time** launch.

**Environment** Development and staging LMS environments.

---

###

### 5.1.4 SMS/Email Notification Gateway ([[3.2.4]{.underline}](#sms-email-gateway-interface))

---

**Methods** Trigger real alerts (test accounts) for various
actions (such as low attendance, fee due). Confirm
delivery status, content accuracy, and user
preference configurations.

---

**Responsibility** QA team and notification service lead.

**Verification During functional testing of alert workflows and any
time** template update.

**Environment** Staging and production with sandbox API keys.

---

### 5.1.5 Authentication Service (SSO/OAuth) Interface ([[3.2.5]{.underline}](#authentication-service-interface))

---

**Methods** Test login with valid and invalid credentials through
the SSO gateway. Validate token generation, session
handling, and role-based dashboard redirection.

---

**Responsibility** QA team and university IT security team.

**Verification At user provisioning rollout and before new semester
time** sessions.

**Environment** Staging and production SSO sandbox environments.

---

### 5.1.6 Payment Gateway Interface ([[3.2.6]{.underline}](#payment-gateway-interface))

---

**Methods** Simulate payment flow using test invoice and validate
payment status updates. Test payment failure
handling, timeout recovery, and transaction logging.

---

**Responsibility** QA team and finance IT representative.

**Verification Before fee collection windows and after API updates
time** from provider.

**Environment** Test sandbox and staging gateway environments (such
as FPX/iPay88 test mode).

---

##

##

##

## 5.2 Verification of Functional Requirements

**5.2.1 User Authentication and
Authorization([[3.4.1.1]{.underline}](#requirement-1))**

---

Methods: Functional testing, penetration testing, MFA validation,
and code review for secure login.

---

Responsibility: Development team and external security consultant.

Verification During development and before production release;
Time: periodic audits post-deployment.

Environment: Development and staging servers.

---

##

**5.2.2 View Academic Grades([[3.4.1.2]{.underline}](#requirement-2))**

---

Methods: Functional testing, data validation checks, and
role-based access testing.

---

Responsibility: QA team.

Verification During system integration testing.
Time:

Environment: Staging environment with test student data.

---

##

**5.2.3 Access Attendance
Records([[3.4.1.3]{.underline}](#requirement-3))**

---

Methods: Functional testing of attendance logs, filters, and
export options.

---

Responsibility: QA team.

Verification Pre-deployment testing.
Time:

Environment: Development and staging environments.

---

##

**5.2.4 Access Academic Timetable
([[3.4.1.4]{.underline}](#requirement-4))**

---

Methods: Usability and functional testing with real-time calendar
integration validation.

---

Responsibility: Product and QA team.

Verification During feature roll-out testing.
Time:

Environment: Development environment and UAT (User Acceptance Testing)
stage.

---

**5.2.5 Manage User Accounts and
Roles([[3.4.1.5]{.underline}](#requirement-5))**

---

Methods: Functional testing for role creation, permissions
handling, and user lifecycle management.

---

Responsibility: Admin module team.

Verification During user management module implementation.
Time:

Environment: Development and admin-controlled test environments.

---

**5.2.6 Integration with Campus
Systems([[3.4.1.6]{.underline}](#requirement-6))**

---

Methods: API integration testing, mock service simulation, and
data sync validation.

---

Responsibility: Integration team.

Verification During system interfacing and staging rollout.
Time:

Environment: Development with mock CLiC, LMS, and CMS endpoints.

---

**5.2.7 Maintain Data Privacy and
Permissions([[3.4.1.7]{.underline}](#requirement-7))**

---

Methods: Role-based access control (RBAC) testing, audit logs, and
compliance checks (PDPA, GDPR).

---

Responsibility: Security compliance team.

Verification Before deployment and during periodic audits.
Time:

Environment: Controlled test environment.

---

**5.2.8 Pay Tuition and Other
Fees([[3.4.1.8]{.underline}](#requirement-8))**

---

Methods: Integration testing with payment gateway and transaction
validation.

---

Responsibility: Backend development and finance integration teams.

Verification After payment module is integrated.
Time:

Environment: Staging environment with sandbox payment credentials.

---

**5.2.9 View Payment History and Invoices
([[3.4.1.9]{.underline}](#requirement-9))**

---

Methods: Functional testing, data accuracy checks, and user
accessibility validation.

---

Responsibility: QA and finance module team.

Verification During post-transaction validation testing.
Time:

Environment: Staging environment.

---

**5.2.10 Upload and Manage
Grades([[3.4.2.1]{.underline}](#requirement-10))**

---

Methods: Functional testing, input validation, bulk upload checks.

---

Responsibility: Lecturer-side QA and dev team.

Verification During internal testing phase.
Time:

Environment: Staging environment with mock class data.

---

**5.2.11 Digital Attendance Tracking
([[3.4.2.2]{.underline}](#requirement-11))**

---

Methods: QR code scanning simulation, manual input testing, record
validation.

---

Responsibility: QA Team

Verification Pre-deployment phase.
Time:

Environment: Mobile emulator and browser staging environment.

---

**5.2.12 Post Announcement and
Updates([[3.4.2.3]{.underline}](#requirement-12))**

---

Methods: Functional testing for announcement creation, user
delivery tracking, and UI feedback.

---

Responsibility: Content and dev team.

Verification After CMS integration.
Time:

Environment: Development and staging server.

---

**5.2.13 Dashboard with Performance
Overview([[3.4.2.4]{.underline}](#requirement-13))**

---

Methods: Visualization rendering test, data aggregation
validation, UI responsiveness testing.

---

Responsibility: Frontend and analytics team.

Verification Post-integration testing phase.
Time:

Environment: UAT and staging.

---

**5.2.14 Submit Feedback and Support
Requests([[3.4.2.5]{.underline}](#requirement-14))**

---

Methods: Form validation, ticket creation flow, and routing logic
testing.

---

Responsibility: Support system team.

Verification Upon internal beta testing.
Time:

Environment: Test helpdesk environment.

---

**5.2.15 Alert and Reminder
System([[3.4.2.6]{.underline}](#requirement-15))**

---

Methods: Notification trigger simulation, queue monitoring,
delivery validation.

---

Responsibility: Backend notification service team.

Verification Before release and during reliability audits.
Time:

Environment: Text messaging environment using Twilio/SMS sandbox

---

**5.2.16 Notification Read
Tracking([[3.4.3.1]{.underline}](#requirement-16))**

---

Methods: User interaction logging test, status flag tracking,
read/unread state toggling.

---

Responsibility: UI/UX telemetry team.

Verification During real-user simulation testing.
Time:

Environment: Staging with event tracking tools.

---

**5.2.17 Custom Notification
Preferences([[3.4.3.2]{.underline}](#requirement-17))**

---

Methods: Preference update test, delivery filter checks, setting
persistence validation.

---

Responsibility: User settings module team.

Verification Pre-launch personalization feature test.
Time:

Environment: Settings sandbox environment.

---

**5.2.18 Visual Performance
Analytics([[3.4.3.3]{.underline}](#requirement-18))**

---

Methods: Graph rendering checks, accuracy tests with mock data,
and responsiveness testing.

---

Responsibility: Data visualization and frontend teams.

Verification After analytics engine integration.
Time:

Environment: Development and analytics testing stage.

---

**5.2.19 Mobile-Friendly Responsive
Interface([[3.4.3.4]{.underline}](#requirement-19))**

---

Methods: Cross-device UI tests, responsive CSS checks, and
accessibility validation (WCAG).

---

Responsibility: UI/UX team.

Verification During frontend QA.
Time:

Environment: Browser stack/mobile testing platforms.

---

##

## 5.3. Verification of Usability Requirements ([[3.6]{.underline}](#usability-requirements))

### 5.3.1 User Interface ([[3.6.1]{.underline}](#user-interface))

**5.3.1.1 Consistent Layout and Design**

---

Methods: Conduct evaluation and consistency checks across modules
to ensure uniform layout.

---

Responsibility: UI/UX team.

Verification During interface design review and at UAT stage.
Time:

Environment: Staging with different user roles

---

##

**5.3.1.2 Responsive Design**

---

Methods: Test portal on desktop, tablet and mobile for layout sync
and functionality

---

Responsibility: Front-end and QA team

Verification During front end testing
Time:

Environment: Multiple browsers and device in staging

---

##

### 5.3.2 User Experience ([[3.6.2]{.underline}](#user-experience))

**5.3.2.1 Efficient Navigation**

---

Methods: Test the quickness of the user to reach key features like
grades and registration. Measure number of clicks and
task time

---

Responsibility: UX and QA teams

Verification During UAT and design review
Time:

Environment: Staging using student and lecturer accounts

---

##

**5.3.2.2 Accessibility and Personalized Experience**

---

Methods: Use screen readers and accessibility tools to test WCAG
2.1 compliance. Check course suggestions and contrast.

---

Responsibility: QA and accessibility team

Verification During UI testing and after updates
Time:

Environment: Staging on various devices and assistive tools

---

##

### 5.3.3 Communication ([[3.6.3]{.underline}](#communication))

**5.3.3.1 Feedback Mechanism**

---

Methods: Check if confirmation or error messages appear after
actions like form submission or uploads.

---

Responsibility: QA and UX teams

Verification During functional testing
Time:

Environment: Staging across key features

---

##

**5.3.3.2 Language Standards**

---

Methods: Review system text for clear, non-technical language in
instructions and alerts.

---

Responsibility: Content reviewer and QA team

Verification During UI review and content proofreading
Time:

Environment: Design and staging environments

---

##

**5.3.3.2 Notification Management**

---

Methods: Test SMS/email settings to ensure users can change
notification preferences.

---

Responsibility: QA and communication integration team.

Verification During integration and UAT.
Time:

Environment: Staging environment with test user roles

---

### 5.3.3 Data Protection ([[3.6.4]{.underline}](#data-protection))

**5.3.4.1 Data Encryption**

---

Methods: Leave session idle and verify if the user is logged out
automatically after the timeout period.

---

Responsibility: QA and security teams.

Verification During security and usability testing.
Time:

Environment: Staging environment with test user sessions.

---

##

**5.3.4.2 Server Controls**

---

Methods: Verify HTTPS is enforced across all pages using browser
dev tools and security scanners.

---

Responsibility: DevOps and security teams.

Verification During deployment and penetration testing.
Time:

Environment: Staging and production environments.

---

##

## 5.4. Verification of Performance Requirements ([[3.5]{.underline}](#performance-requirements))

### 5.4.1 Static Numerical Requirements ([[3.5.1]{.underline}](#static-numerical-requirements))

**5.4.1.1 Storage Scalability**

---

Methods: Test storage handling with mock academic and media data
to reach 2TB. Check backup interval and recovery time.

---

Responsibility: QA and DevOps teams.

Verification During performance testing.
Time:

Environment: Staging with real-time load simulation.

---

##

**5.4.1.2 Database Backups**

---

Methods: Check data backup storage allocation every 12 hours for
data tracking and retrieval

---

Responsibility: DevOps and security teams

Verification During performance testing.
Time:

Environment: Staging with real-time load simulation.

---

##

**5.4.1.3 Data Retrieval Speed**

---

Methods: Send multiple queries for student records, schedules, and
attendance, and measure response time.

---

Responsibility: QA teams.

Verification During performance testing.
Time:

Environment: Staging with real-time load simulation.

---

##

**5.4.1.4 Simultaneous User Capacity**

---

Methods: Simulate 5,000 users performing key actions. Monitor
system load, latency, and crash reports.

---

Responsibility: Performance and QA teams.

Verification During stress testing and scalability evaluation.
Time:

Environment: Load testing tools in a staging environment.

---

##

**5.4.1.4 Session Timeout**

---

Methods: Leave sessions inactive for 15 minutes and verify auto
logout and session data clearance.

---

Responsibility: QA and security team

Verification During security and usability testing.
Time:

Environment: Staging with role-based test users.

---

##

### 5.4.1 Dynamic Numerical Requirements ([[3.5.2]{.underline}](#dynamic-numerical-requirements))

**5.4.1.1 Task Handling**

---

Methods: Task completion analysis on automated log sand error rate
reports

---

Responsibility: Performance and QA teams

Verification During performance and integration testing
Time:

Environment: Staging environment with simulated data loads and
automation triggers

---

**5.4.1.2 System Uptime**

---

Methods: Deploy system monitoring using uptime tracking tools.
Simulate failure and recovery scenarios.

---

Responsibility: DevOps team

Verification Post-deployment monitoring
Time:

Environment: Pre-production staging with simulated failover

---

**5.4.1.3 Feature Responsiveness**

---

Methods: Perform response time tests on core modules with
simulated user actions.

---

Responsibility: QA Team

Verification Performance Testing
Time:

Environment: Staging with simulated user workflows

---

##

**5.4.1.4 Background Data Synchronization**

---

Methods: mock synchronization events between systems using
simulated updates.

---

Responsibility: Integration QA Team

Verification During data testing
Time:

Environment: Staging with real-time sync simulators

---

##

**5.4.1.5 Grade Upload Processing**

---

Methods: test grade files with varied data types and formats.
Monitor system logs and error handling reports to confirm
error-free processing

---

Responsibility: QA Team

Verification Data Handling Test Phase
Time:

Environment: Staging environment with simulated academic records

---

##

**5.4.1.5 Report Generation**

---

Methods: Generate reports with test data under standard usage. Log
and analyze response time per report

---

Responsibility: QA Team

Verification Functional and Load Testing
Time:

Environment: staging with typical usage patterns and academic datasets

---

##

**5.4.1.6 Peak load Response Time**

---

Methods: load testing tools to simulate concurrent users executing
various tasks. Measure response times and confirm less
than 10% of total requests are delayed or failed.

---

Responsibility: Performance Team

Verification Stress and Load Testing Phase
Time:

Environment: Scaled staging environment replicating peak university
usage

---

##

**5.4.1.7 Transaction Processing**

---

Methods: Simulate transactions for login, course enrollment, and
grade input. Track completion times and validate

---

Responsibility: QA and BAck-end Team

Verification Functional Performance Testing
Time:

Environment: Staging with emulated normal daily user activity

---

##

## 5.5. Verification of Logical Database Requirements ([[3.8]{.underline}](#logical-database-requirements))

### 5.5.1 Data Integrity Enforcement

---

Methods: Test insertion, update, and deletion of records to
confirm enforcement of constraints (e.g., NOT NULL,
UNIQUE, CHECK). Validate business rules through automated
test cases.

---

Responsibility: Database developers and QA team.

Verification During integration testing and database testing phases.
Time:

Environment: Staging database environment with mock academic datasets.

---

##

### 5.5.2 Referential Integrity Checks

---

Methods: Execute queries that involve foreign key relationships to
ensure cascading updates/deletes behave correctly.
Attempt violations to test constraint enforcement.

---

Responsibility: QA and database administration teams.

Verification During schema validation and functional database testing.
Time:

Environment: Controlled staging database with test relationships.

---

##

### 5.5.3 Normalization Compliance

---

Methods: Review schema design for adherence to at least 3NF.
Conduct manual and automated checks for redundancy and
anomalies in table structures.

---

Responsibility: Database architects and QA reviewers.

Verification During design and code review stages.
Time:

Environment: Database design documentation and test schema review
environment.

---

##

### 5.5.4 Query Accuracy and Performance

---

Methods: Execute frequently used queries (e.g., fetch student
records, schedules, attendance) to validate data
correctness and acceptable execution time (\< 2 seconds
for most queries).

---

Responsibility: QA and performance teams.

Verification During performance and UAT testing phases.
Time:

Environment: Staging environment with realistic data volumes.

---

##

### 5.5.5 Data Redundancy Detection

---

Methods: Use SQL scripts to identify duplicate entries in key
tables (e.g., student profiles, course lists). Monitor
ETL processes to avoid redundant data insertion.

---

Responsibility: Data engineering and QA team.

Verification During integration and data migration testing.
Time:

Environment: Staging environment with migration datasets.

---

### 5.5.6 Transactional Consistency (ACID Properties)

---

Methods: Simulate multi-step transactions (e.g., student
enrollment and payment) to ensure atomicity, consistency,
isolation, and durability.

---

Responsibility: Backend development and QA teams.

Verification During database transaction testing and security testing.
Time:

Environment: Staging environment with transactional logs enabled.

---

### 5.5.7 Backup and Recovery Validation

---

Methods: Trigger backup creation and simulate failure scenarios to
ensure database restoration maintains logical integrity
(e.g., no orphaned records or corruption).

---

Responsibility: DevOps and DBA teams.

Verification During disaster recovery drills and release cycles.
Time:

Environment: Backup/recovery sandbox with versioned snapshots.

---

##

## 5.6. Verification of Design Constraints ([[3.9]{.underline}](#design-constraints))

### 5.6.1 Compliance with Data Privacy Regulations ([[3.9.1]{.underline}](#compliance-with-data-privacy-regulations))

---

**Methods** Conduct documentation review and technical tests to
ensure compliance with PDPA. Simulate scenarios for
personal data access and validate encryption and
consent enforcement.

---

**Responsibility** Compliance officer and product team.

**Verification During the requirements definition, testing, and
time** before production rollout.

**Environment** Development, staging, and remote documentation
environments.

---

### 5.6.2 Integration with Existing University Systems ([[3.9.2]{.underline}](#integration-with-existing-university-systems))

---

**Methods** Perform API contract testing with CLiC and LMS.
Conduct data mapping verification and simulate
student data sync flows to ensure field
compatibility.

---

**Responsibility** Integration lead and product team.

**Verification During API integration phase and post-deployment
time** patches.

**Environment** Staging and production sandbox environments.

---

### 5.6.3 Security Standards ([[3.9.3]{.underline}](#security-standards))

---

**Methods** Run OWASP-based security scans, static code analysis,
and penetration tests. Validate token expiry,
password encryption, and XSS/SQL injection
protection.

---

**Responsibility** Security team and QA testers.

**Verification Before each deployment cycle and during security
time** audits.

**Environment** Staging and vulnerability assessment environments.

---

### 5.6.4 Accessibility Requirements ([[3.9.4]{.underline}](#accessibility-requirements))

---

**Methods** Use tools such as WAVE, aXe, and manual tab testing
to validate keyboard navigation, alt text, ARIA
labels, and color contrast as per WCAG 2.1 standards.

---

**Responsibility** UI/UX designers and QA team.

**Verification During front-end development and UI freeze.
time**

**Environment** Cross-browser test environments and accessibility
tools.

---

### 5.6.5 API Usage Limitations ([[3.9.5]{.underline}](#api-usage-limitations))

---

**Methods** Simulate multiple API calls using Postman and Locust
to verify API rate limits and retry mechanisms.
Confirm request throttling for SMS gateway and
payment APIs.

---

**Responsibility** Backend devs and QA testers.

**Verification During API testing and before system stress tests.
time**

**Environment** Staging and pre-production integration environments.

---

### 5.6.6 Performance and Scalability ([[3.9.6]{.underline}](#performance-and-scalability))

---

**Methods** Use JMeter and k6 to simulate 500+ concurrent logins,
grade queries, and SMS triggers. Measure response
time and memory consumption under stress.

---

**Responsibility** Performance engineering team.

**Verification Before semester starts or exam periods.
time**

**Environment** Performance test server environment.

---

### 5.6.7 User Experience Consistency ([[3.9.7]{.underline}](#user-experience-consistency))

---

**Methods** Conduct usability testing with real users on phones,
tablets, and desktops. Use BrowserStack to test
consistency across Chrome, Firefox, Safari.

---

**Responsibility** UI/UX team and QA.

**Verification During front-end iterations and usability evaluation.
time**

**Environment** Responsive browser/device test lab.

---

### 5.6.8 Data Interoperability ([[3.9.8]{.underline}](#data-interoperability))

---

**Methods** Check that all integrated systems send/receive JSON
objects according to API documentation. Validate
encoding, timestamp formats, and key consistency.

---

**Responsibility** Integration devs and QA team.

**Verification During data flow tests and third-party integrations.
time**

**Environment** Staging systems and integration endpoints.

---

### 5.6.9 Legal and Ethical Considerations ([[3.9.9]{.underline}](#legal-and-ethical-considerations))

---

**Methods** Verify audit trail coverage, data consent logs, and
compliance features for student rights to data access
and deletion.

---

**Responsibility** Legal liaison and product owner.

**Verification During requirements finalization and before go-live.
time**

**Environment** Documentation review and simulated compliance
environment.

---

### 5.6.10 Project Budget and Timeline ([[3.9.10]{.underline}](#project-budget-and-timeline))

---

**Methods** Use Gantt charts and financial logs to track project
milestones and budget variance. Perform monthly
reviews with the PMO.

---

**Responsibility** Project manager and finance representative.

**Verification Continuously across all project phases.
time**

**Environment** Project management dashboard and cost tracking
system.

---

## 5.7 Verification of Software System Attributes ([[3.10]{.underline}](#software-system-attributes))

**5.7.1 Reliability ([[3.10.1]{.underline}](#reliability))**

---

Methods: Stress testing, reliability testing, data integrity
validation, backup and recovery drills

---

Responsibility: QA team

Verification Post implementation, pre-deployment
time:

Environment: Staging environment

---

**5.7.2 Availability ([[3.10.2]{.underline}](#availability))**

---

Methods: Load testing, redundancy testing, monitoring validation

---

Responsibility: QA team

Verification Post implementation, pre-deployment
time:

Environment: Staging environment

---

**5.7.3 Security ([[3.10.3]{.underline}](#security-1))**

---

Methods: Penetration testing, code review, cryptographic
validation, logging audits

---

Responsibility: Security team and external auditors

Verification Pre-deployment and periodic reviews
time:

Environment: Staging and production environments

---

**5.7.4 Maintainability ([[3.10.4]{.underline}](#maintainability))**

---

Methods: Code review, modularity analysis, bug tracking audit

---

Responsibility: Development and QA teams

Verification Throughout deployment and pre-deployment
time:

Environment: Development environment

---

**5.7.4 Portability ([[3.10.5]{.underline}](#portability))**

---

Methods: Cross-platform testing, Docker/containerization testing

---

Responsibility: Development and QA teams

Verification Testing phase post-implementation
time:

Environment: Staging environment on multiple OS platforms

---

#

# 6. Appendices

## 6.1 Assumptions and dependencies

#### Assumptions:

1.  The system shall have pre-registered parent, student, and admin
    accounts with verified email and phone numbers.

2.  The system shall be accessible via modern internet browsers (e.g.,
    Chrome, Firefox, Edge).

3.  The system shall have a list of FCI students and their academic
    records preloaded in the database.

4.  The system shall store parent-student relationship mappings within
    the database.

5.  The system shall support English language as the primary language
    interface.

6.  The system shall have integrated notification services (SMS/Email
    API) properly configured.

#### Dependencies:

1.  The system shall require a stable internet connection for both
    clients and servers.

2.  The system shall require a device with an internet browser (desktop,
    tablet, or mobile).

3.  The system shall depend on third-party email and SMS gateways (e.g.,
    SMTP, Twilio) for alert delivery.

4.  The system shall depend on a relational database (e.g.,
    MySQL/PostgreSQL) to store and manage user and academic data.

5.  The system shall rely on authentication mechanisms (e.g., JWT or
    OAuth2) to validate users and maintain session security.

## 6.2 Acronyms and abbreviations

1.  CliC: Campus Life and Information Centre

2.  SMS: Short Message Service

3.  JSON: JavaScript Object Notation

4.  UCSP: University Communication and Service Portal

5.  IT: Information Technology

6.  LMS: Learning Management System

7.  CMS: Campus Management System

8.  API: Application Programming Interface

9.  MFA: Multi-Factor Authentication

10. SSO: Single Sign-On

11. CRUD: Create,Read,Update,Delete

12. UI: User Interface

13. UX: User Experience

14. HTTPS: HyperText Transfer Protocol Secure

15. GDPR: General Data Protection Regulation

16. PDPA: Personal Data Protection Act(Malaysia)

17. REST: Representational State Transfer

18. DBMS: Database Management System

19. SQL: Structured Query Language

20. SSL: Secure Sockets Layer

21. WCAG: Web Content Accessibility Guidelines

22. LTS: Long-Term Support

23. SMTP: Simple Mail Transfer Protocol

24. RFC: Request for Comments

25. MIME: Multipurpose Internet Mail Extensions

26. HTML: HyperText Markup Language

27. RAM: Random Access Memory

28. RTO: Recovery Time Objective

29. LDAP: Lightweight Directory Access Protocol

30. ID: Identifier

31. AWS: Amazon Web Services

32. GCP: Google Cloud Platform

33. ERP: Enterprise Resource Planning

34. MMU: Multimedia University

35. MVP: Minimum Viable Product

36. OWASP: Open Worldwide Application Security Project

37. ACID: Atomicity, Consistency, Isolation, Durability

38. TLS: Transport Layer Security

39. RBAC: Role-Based Access Control

40. UAT: User Acceptance Testing

##

## 6.3 Glossary

1.  Authentication: Process of verifying identity of a user/system.

2.  Auth Service: Service that handles user authentication

3.  Twilio: Cloud platform for SMS, voice, and messaging APIs.

4.  Cache: Temporary storage for frequently accessed data to improve
    speed.

5.  PostGreSQL: Open-source relational database system

6.  Containerization: Packaging software and dependencies into isolated
    units

7.  Cryptographic: Related to cryptography, techniques for secure
    communication.
