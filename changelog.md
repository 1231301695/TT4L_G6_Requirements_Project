# changelog.md – EduAxis SRS

## Content Changes
### CHG-01 – Clarified Memory Requirements and Removed Design-Level Details  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: REQ-01  
Session ID: VS-01  
Sections Affected: 1.3.1.6 Memory Constraints

**What Changed/Added**:  
- Replaced general description with a clear, measurable requirement:  
  - "The system must support up to 5,000 concurrent users with a maximum RAM consumption of 16 GB."  
- Removed low-level implementation explanations (e.g., caching and session memory handling).  
- Mentioned that technical details will be handled later in the design documentation.

**Why It Was Changed/Added**:  
The original section described memory behavior at an implementation level (e.g., how caching works, session memory use), which does not belong in an SRS.

**Impact**:  
- Makes the requirement measurable for testing.  
- Shifts design decisions (like caching) to the appropriate phase.  
- Clarifies expectations for system scalability during development.


### CHG-02 – Added Minimum Server Specs  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: REQ-02  
Session ID: VS-01  
Sections Affected: 1.3.1.3 Hardware Interfaces

**What Changed/Added**:  
- Added deployment server specs:
  - Minimum: 4-core CPU, 8 GB RAM, 256 GB SSD
- Mentioned that these specs are to support high concurrency and real-time data sync.

**Why It Was Changed/Added**:  
- The section had no hardware guidance, which could lead to unclear system expectations or deployment delays.

**Impact**:  
- Helps infrastructure teams plan for deployment.  
- Provides a baseline to evaluate system load handling.  
- Makes the hardware environment reproducible and consistent across institutions.



### CHG-03 – Added Bandwidth and Latency Requirements  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: REQ-04  
Session ID: VS-01  
Sections Affected: 1.3.1.5 Communication Interfaces

**What Changed/Added**:  
- Defined expected network performance:
  - 5 Mbps minimum client bandwidth  
  - 100 Mbps minimum server bandwidth  
  - Max 100 ms latency for alert delivery  
- Included support for both cloud-based and on-campus network access.

**Why It Was Changed/Added**:  
- Without these numbers, the system’s network performance expectations were unclear.  
- Real-time features (notifications, sync) require specific thresholds to function properly.

**Impact**:  
- Makes communication performance measurable during testing.  
- Ensures the system works reliably in real-time scenarios.  
- Supports capacity planning for university IT teams.




### CHG-04 – Standardized Product Name to “EduAxis”  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: REQ-05  
Session ID: VS-01  
Sections Affected: 1.1 Purpose, General References

**What Changed/Added**:  
- Replaced inconsistent naming (“UCSP” and “EduAxis”) with a single, unified name: **EduAxis**.  
- Updated all references to use the brand name consistently across the document.

**Why It Was Changed/Added**:  
- Stakeholders and the marketing team confirmed that "EduAxis" is the official product name.  
- Having two names in the document was confusing and didn’t align with branding guidelines.

**Impact**:  
- Improves document clarity and professionalism.  
- Reduces reader confusion during stakeholder reviews.  
- Aligns SRS content with official communication and UI naming.




### CHG-05 – Standardized Accessibility Requirement Terminology  
Date: 2025-06-20  
Proposed By: Tan Jun Xian, Soukmaed Ong Yu Kang, Loqman  
Req ID: REQ-06  
Session ID: VS-02  
Sections Affected: 1.3.1, 3.6.2, 3.9.4, 3.9.11.4, 5.3.2.2

**What Changed/Added**:  
- Replaced general mentions of “accessibility” with the formal standard: **WCAG 2.1 Level AA**.  
- Applied consistently across all relevant sections, aligning with Section 3.6.2.

**Why It Was Changed/Added**:  
- “Accessibility” was too broad and inconsistently applied. Using a specific standard removes ambiguity and improves compliance clarity.

**Impact**:  
- Improves clarity for developers and testers.  
- Ensures accessibility goals are aligned with recognized global standards.  
- Makes the requirement auditable and consistent across the SRS.




### CHG-06 – Added Storage Capacity Limit and Scaling Strategy  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: REQ-07  
Session ID: VS-02  
Sections Affected: 3.5.1

**What Changed/Added**:  
- Added a **10 TB maximum** storage limit to complement the existing **2 TB minimum**.  
- Described a basic scaling strategy to guide system growth.

**Why It Was Changed/Added**:  
- Only a lower bound was mentioned before. The update provides a more realistic boundary and planning guidance for future system use.

**Impact**:  
- Helps capacity planning for infrastructure teams.  
- Sets a clearer benchmark for when storage expansion is needed.  
- Makes the system more maintainable as usage increases.



### CHG-07 – Listed Specific Security Measures  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: REQ-08  
Session ID: VS-03  
Sections Affected: 3.9.3, 3.10.3.1

**What Changed/Added**:  
- Replaced generic mention of “OWASP guidelines” with a list of actual security practices:  
  - Password encryption  
  - Secure login  
  - User activity logging

**Why It Was Changed/Added**:  
- The old version was vague. The updated list gives clear expectations of what security features will be implemented.

**Impact**:  
- Makes the security plan more understandable for developers.  
- Enables clear testing for security compliance.  
- Helps match security requirements to institutional IT policies.



### CHG-08 – Defined Connection Interface Requirements  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: REQ-09  
Session ID: VS-03  
Sections Affected: 3.9.2

**What Changed/Added**:  
- Defined the exact technologies to be used for system communication:
  - RESTful APIs  
  - JSON as the data format  
  - HTTPS for all external/internal communication

**Why It Was Changed/Added**:  
- The old version just said the system "connects to other systems" with no technical context. This change makes it actionable and understandable for API developers.

**Impact**:  
- Reduces uncertainty for integration and third-party developers.  
- Sets a baseline for interface design and security expectations.  
- Supports alignment with modern web standards.



### CHG-09 – Resolved Incomplete Budget Constraint  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: REQ-10  
Session ID: VS-03  
Sections Affected: 3.9.1, 3.9.10

**What Changed/Added**:  
- Removed phrases like “budget constraints” that were unsupported by actual values or estimates.

**Why It Was Changed/Added**:  
- Vague budget references without numbers added confusion. This change keeps the SRS focused on what can be specified or tested.

**Impact**:  
- Reduces ambiguity in financial expectations.  
- Prevents miscommunication between clients and developers.  
- Keeps the SRS within its scope (technical, not financial planning).



### CHG-10 – Added Failure Test Cases for Edge Scenarios  
Date: 2025-06-20  
Proposed By: Loqman  
Req ID: REQ-11  
Session ID: VS-04  
Sections Affected: 5.2.1, 5.2.8

**What Changed/Added**:  
- Included failure-based test cases for:
  - Login failure  
  - Payment timeouts  
  - Invalid user input

**Why It Was Changed/Added**:  
- The test plan only covered expected, successful flows. These additions improve error handling validation.

**Impact**:  
- Improves system reliability and robustness.  
- Helps QA teams cover edge cases.  
- Ensures better user experience in real-world use.



### CHG-11 – Clarified Legal Compliance Test for Data Deletion  
Date: 2025-06-20  
Proposed By: Loqman  
Req ID: REQ-12  
Session ID: VS-05  
Sections Affected: 5.6.9 Legal & Ethical

**What Changed/Added**:  
- Added a validation method to confirm the system complies with “right to be forgotten” regulations.  
- Included examples like data deletion workflows, audit logs, and confirmation screens.

**Why It Was Changed/Added**:  
- The section previously mentioned legal compliance without explaining how it would be tested or validated.

**Impact**:  
- Improves traceability of legal features.  
- Provides clear test cases for compliance audits.  
- Helps ensure regulatory readiness for data privacy laws.



### CHG-12 – Added Explanation of Assumptions and Their Impact  
Date: 2025-06-20  
Proposed By: Lai Joon Li  
Req ID: REQ-13  
Session ID: VS-05  
Sections Affected: 6.1 Assumptions

**What Changed/Added**:  
- For each assumption listed, added a short explanation describing how it could affect system functionality, reliability, or implementation.

**Why It Was Changed/Added**:  
- The assumptions were previously listed with no context, which made it hard to evaluate their risks or relevance.

**Impact**:  
- Helps stakeholders understand limitations and boundaries.  
- Clarifies risk areas for planning and development.  
- Improves the document’s completeness and usefulness.




### CHG-13 – Added Explanation of RESTful API Reference  
Date: 2025-06-20  
Proposed By: Lai Joon Li  
Req ID: REQ-14  
Session ID: VS-05  
Sections Affected: 6.3 Future Work

**What Changed/Added**:  
- Briefly explained what RESTful APIs are and how they relate to future system integration plans.

**Why It Was Changed/Added**:  
- REST API was mentioned without any explanation, which could confuse non-technical readers or new developers.

**Impact**:  
- Improves clarity of the Future Work section.  
- Provides better direction for future development planning.  
- Makes the document easier to understand for broader audiences.



### CHG-14 – Added Technical Configuration for University Academic Data  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: REQ-15  
Session ID: VS-06  
Sections Affected: 1.3.1.8 Configuration

**What Changed/Added**:  
- Added specific parameters for configuring:
  - Academic calendars (semester, trimester, quarter)  
  - Grading scales (4.0 GPA, percentage, letter grades)  
  - Course code structures (e.g., CS101, MATH-202A)  
  - Integration templates (LDAP, OAuth, Active Directory)

**Why It Was Changed/Added**:  
- The original text was too vague about what was configurable. This change provides clear, structured examples.

**Impact**:  
- Makes the system’s flexibility and adaptability easier to implement.  
- Supports university-specific customization.  
- Improves traceability of configurable modules.



### CHG-15 – Defined Foreign Key Constraints and Behavior  
Date: 2025-06-20  
Proposed By: Loqman  
Req ID: REQ-16  
Session ID: VS-06  
Sections Affected: 3.7.7 Database Constraints

**What Changed/Added**:  
- Defined foreign key behaviors:
  - CASCADE for grade deletion when a course is removed  
  - RESTRICT for student deletion when grades exist  
  - SET NULL for lecturer replacement  
- Added:
  - CHECK constraints (e.g., grade range 0–100)  
  - UNIQUE constraints (student-course-semester combo)  
  - Parent-student relationship rules

**Why It Was Changed/Added**:  
- There were no rules defining how relationships should behave during deletion or update. These additions ensure data consistency.

**Impact**:  
- Improves data integrity and reliability.  
- Supports safe handling of relational data during updates or deletions.  
- Reduces the chance of unintended data loss or logic errors.



### CHG-16 – Defined Severity Levels and Escalation Flow  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: REQ-17  
Session ID: VS-06  
Sections Affected: 3.10.4.3 Incident Management

**What Changed/Added**:  
- Added definitions for issue severity:
  - Critical (system down, respond <2 hrs)  
  - High (major feature issue, <8 hrs)  
  - Medium (minor issue, <48 hrs)  
  - Low (cosmetic, <1 week)  
- Added:
  - Escalation path  
  - Communication flow  
  - Priority matrix by user impact

**Why It Was Changed/Added**:  
- Severity levels were mentioned but never defined. This creates a formal response process for incident management.

**Impact**:  
- Ensures faster and more predictable issue resolution.  
- Aligns team expectations during live system maintenance.  
- Improves user trust in platform support.



### CHG-17 – Added Fallback Actions for Throttling  
Date: 2025-06-20  
Proposed By: Lai Joon Li  
Req ID: REQ-18  
Session ID: VS-06  
Sections Affected: 3.9.5 Performance Constraints

**What Changed/Added**:  
- Added fallback logic to handle throttling:
  - Exponential backoff (1s, 2s, 4s, 8s)  
  - HTTP 429 response with Retry-After header  
  - Queueing low-priority tasks  
  - User notifications during degraded performance  
  - Priority queue for critical functions (e.g., attendance)

**Why It Was Changed/Added**:  
- Throttling was too vague. These updates show how the system should respond under stress.

**Impact**:  
- Improves system stability under load.  
- Enhances user experience during peak periods.  
- Helps developers implement graceful degradation.



### CHG-18 – Added SMS Length Limit Handling  
Date: 2025-06-20  
Proposed By: Loqman  
Req ID: REQ-19  
Session ID: VS-06  
Sections Affected: 1.3.1.5 Communication Interfaces

**What Changed/Added**:  
- Clarified how to handle SMS message limits:
  - Split messages over 160 characters  
  - Support for international number formats (+60, +1, etc.)

**Why It Was Changed/Added**:  
- SMS functionality was included, but technical limitations like character limits and formatting were not addressed.

**Impact**:  
- Prevents message cutoff or delivery failure.  
- Ensures international compatibility and compliance.  
- Improves reliability of communication with users.

---

## Document Changes
### CHG-19 – Added Stakeholder Expectations in Purpose and Scope  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: - 
Session ID: VS-01  
Sections Affected: Pages 6–7

**What Changed/Added**:  
- Added a short summary of stakeholder needs under both Purpose and Scope sections:  
  - Students want centralized access to academic records, grades, and schedules  
  - Parents want performance alerts and fee notifications  
  - Lecturers need course and grading tools  
  - Admins require system control, reporting, and helpdesk capabilities

**Why It Was Changed/Added**:  
- The original version did not mention what different users expect from the system. Including this helps tie the project goals to actual user needs.

**Impact**:  
- Improves alignment between user requirements and system objectives  
- Helps stakeholders see their needs reflected in the document  
- Provides context for the system’s feature set and design priorities



### CHG-20 – Rewrote Long Paragraphs for Better Readability  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: -  
Session ID: VS-01  
Sections Affected: Pages 8, 9, 10, 13

**What Changed/Added**:  
- Split up long blocks of text into shorter, clearer paragraphs.  
- Rephrased complex wording into simpler, more readable sentences.

**Why It Was Changed/Added**:  
- The original writing was dense and hard to follow, especially for non-technical readers.

**Impact**:  
- Improves document readability and flow.  
- Makes the SRS more user-friendly for all stakeholders and team members.



### CHG-21 – Standardized Use Case Table Formatting  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: -  
Session ID: VS-01  
Sections Affected: Page 26

**What Changed/Added**:  
- Adjusted all use case tables to have consistent formatting.  
- Ensured actor names (e.g., “Management”) were applied uniformly.

**Why It Was Changed/Added**:  
- Inconsistent table formatting made the document look unpolished and could cause confusion.

**Impact**:  
- Improves professionalism of the SRS.  
- Makes it easier for reviewers to compare use cases across sections.



### CHG-22 – Unified LMS Terminology to “eBwise”  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang, Tan Jun Xian  
Req ID: -  
Session ID: VS-01  
Sections Affected: Throughout Document

**What Changed/Added**:  
- Replaced mixed terms ("LMS", "Learning Management System", "eBwise") with consistent usage.  
- First mention updated to “eBwise (LMS)”, then referred to as “eBwise” throughout.

**Why It Was Changed/Added**:  
- Using three different terms for the same system was confusing and inconsistent.

**Impact**:  
- Improves clarity and branding consistency.  
- Makes it easier to track references to the LMS across the document.



### CHG-23 – Moved Use Case and Interface Sections to the Correct Location  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang, Tan Jun Xian  
Req ID: -  
Session ID: VS-01  
Sections Affected: Pages 9–18 (Section 1.3.2)

**What Changed/Added**:  
- Moved the following content from Section 1.3.2 to Section 3.1:
  - Use Case diagram and table  
  - System Interface  
  - Hardware Interface  
  - Software Interface  
  - Communication Interfaces

**Why It Was Changed/Added**:  
- These sections were incorrectly placed in the Introduction section. SRS structure (IEEE standard) requires them under Functional Requirements.

**Impact**:  
- Aligns document structure with industry standards.  
- Helps reviewers find content in the correct context.  
- Avoids confusion during traceability and validation.



### CHG-24 – Corrected Spelling and Grammar Errors  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang, Lai Joon Li, Loqman  
Req ID: -  
Session ID: VS-01  
Sections Affected: Pages 6–10, 28, 63, 128–132, 160, 165

**What Changed/Added**:  
- Fixed spelling and grammar issues throughout the document (e.g., “LinkdIn” → “LinkedIn”).  
- Cleaned up sentence structures where awkward phrasing was found.

**Why It Was Changed/Added**:  
- Minor errors disrupted readability and professionalism of the document.

**Impact**:  
- Improves the polish and credibility of the SRS.  
- Makes the document easier to read for all audiences.



### CHG-25 – Reformatted References to APA Style  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: -  
Session ID: VS-01  
Sections Affected: Page 94

**What Changed/Added**:  
- Reformatted the reference list to match APA 7th edition style:
  - Italicized source titles  
  - Used correct capitalization, punctuation, and author formatting

**Why It Was Changed/Added**:  
- The references didn’t follow a formal citation format, which could reduce academic validity.

**Impact**:  
- Ensures consistency and professionalism  
- Improves traceability of cited sources  
- Aligns with standard academic requirements



### CHG-26 – Justified Text Formatting Throughout Document  
Date: 2025-06-20  
Proposed By: Lai Joon Li, Tan Jun Xian, Soukmaed Ong Yu Kang  
Req ID: -  
Session ID: VS-01  
Sections Affected: Entire Document

**What Changed/Added**:  
- Aligned all body text to “Justify” for consistency in layout and visual presentation.

**Why It Was Changed/Added**:  
- The previous formatting was uneven, with left-aligned, ragged-right paragraphs.

**Impact**:  
- Enhances document readability and visual professionalism.  
- Ensures alignment consistency in printing and PDF formats.



### CHG-27 – Renumbered All Tables Consistently  
Date: 2025-06-20  
Proposed By: Tan Jun Xian, Soukmaed Ong Yu Kang, Loqman  
Req ID: -  
Session ID: VS-01  
Sections Affected: Pages 66, 112–117, 157, 159–161, 167–168

**What Changed/Added**:  
- Corrected inconsistent table numbers (e.g., “Table A” or duplicates).  
- Applied standard numbering format (Table 3.1, 3.2, etc.) across all sections.

**Why It Was Changed/Added**:  
- Some tables were either misnumbered or skipped, making cross-referencing unclear.

**Impact**:  
- Makes the document easier to navigate.  
- Improves referencing accuracy in discussions and traceability.



### CHG-28 – Standardized Requirement ID Format in Allocation Section  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: -  
Session ID: VS-02  
Sections Affected: Pages 95–96

**What Changed/Added**:  
- Updated unclear requirement IDs to a consistent format: `REQ-001`, `REQ-002`, etc.

**Why It Was Changed/Added**:  
- The original IDs were inconsistently named or incomplete, which made tracking hard.

**Impact**:  
- Makes requirement mapping cleaner for traceability.  
- Improves alignment with industry-standard documentation practices.



### CHG-29 – Added Missing Table Numbers  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: -  
Session ID: VS-02  
Sections Affected: Pages 95–99, 101–107, 120–122, 127–133, 149–168

**What Changed/Added**:  
- Added missing table numbers using the proper format (e.g., Table 3.4, Table 4.1).

**Why It Was Changed/Added**:  
- Many tables were unlabeled or inconsistently numbered, making referencing difficult.

**Impact**:  
- Improves structure and consistency in layout.  
- Helps reviewers and developers easily refer to specific content.



### CHG-30 – Added Missing Figure Numbers  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: -  
Session ID: VS-02  
Sections Affected: Pages 134–142

**What Changed/Added**:  
- Numbered all previously unnumbered figures using the correct format (e.g., Figure 4.1, 4.2, etc.).

**Why It Was Changed/Added**:  
- Several figures were missing identifiers, which caused issues during validation and navigation.

**Impact**:  
- Makes visual references traceable.  
- Improves professionalism and usability of the document.



### CHG-31 – Added Missing Figure References in Text  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: -  
Session ID: VS-02  
Sections Affected: Page 111

**What Changed/Added**:  
- Added figure numbers and proper in-text citations where figures were mentioned but not referenced clearly.

**Why It Was Changed/Added**:  
- Figures were listed or described without being numbered or cited, breaking traceability.

**Impact**:  
- Ensures all visual content is properly documented.  
- Improves clarity for both readers and evaluators.



### CHG-32 – Added HTTPS Validation Method  
Date: 2025-06-20  
Proposed By: Loqman  
Req ID: -  
Session ID: VS-04  
Sections Affected: Page 158 (Section 5.3.4.2)

**What Changed/Added**:  
- Updated the method description to include a clear validation approach for HTTPS:  
  - Use browser DevTools to check SSL certificates  
  - Use an online SSL scanner to verify certificate validity and HTTPS enforcement

**Why It Was Changed/Added**:  
- The original method section mentioned HTTPS as a requirement but didn’t explain how to test or confirm it.

**Impact**:  
- Makes the validation approach specific and testable  
- Helps QA teams confirm security configurations during deployment  
- Strengthens credibility of the security testing phase



### CHG-32 – Added HTTPS Validation Method  
Date: 2025-06-20  
Proposed By: Loqman  
Req ID: -  
Session ID: VS-04  
Sections Affected: Page 158 (Section 5.3.4.2)

**What Changed/Added**:  
- Updated the method description to include a clear validation approach for HTTPS:  
  - Use browser DevTools to check SSL certificates  
  - Use an online SSL scanner to verify certificate validity and HTTPS enforcement

**Why It Was Changed/Added**:  
- The original method section mentioned HTTPS as a requirement but didn’t explain how to test or confirm it.

**Impact**:  
- Makes the validation approach specific and testable  
- Helps QA teams confirm security configurations during deployment  
- Strengthens credibility of the security testing phase



### CHG-33 – Fixed Capitalisation and Spacing in Method Descriptions  
Date: 2025-06-20  
Proposed By: Loqman  
Req ID: -  
Session ID: VS-04  
Sections Affected: Page 161 (Sections 5.4.1.4 – 5.4.1.7)

**What Changed/Added**:  
- Corrected lowercase sentence starts in 5.4.1.4 to 5.4.1.7  
- Removed double spacing in 5.4.1.5 and 5.4.1.7

**Why It Was Changed/Added**:  
- Basic formatting issues were affecting the readability and consistency of the test methods.

**Impact**:  
- Improves document quality and attention to detail  
- Keeps formatting consistent with the rest of the section  
- Makes the content clearer and easier to present or print

---

## Agreement Changes
### CHG-34 – Resolved Conflict on Authentication Method  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: REQ-19  
Session ID: VS-02  
Sections Affected: Authentication Design (Refer to 3.7.9, 3.9.6)

**What Changed/Added**:  
- Documented final agreement to implement centralized **SSO with MFA** using OAuth 2.0, while still supporting username/password for basic services during fallback scenarios.  
- Clarified login flows to balance usability and security:
  - Primary login via SSO (university portal)  
  - MFA enforced for admin and sensitive access  
  - Fallback basic login with internal validation allowed for select cases (e.g., parent portal or mobile app offline mode)

**Why It Was Changed/Added**:  
- There was a conflict between three stakeholders:
  - **Students** wanted simple login with ID and password  
  - **Security team** required MFA and OAuth  
  - **Technical team** had already implemented SSO integration only  
- This compromise ensures system security while acknowledging student usability concerns.

**Impact**:  
- Improves user experience while meeting security policies  
- Prevents future design rollback by aligning with technical constraints  
- Provides clear documentation for system behavior in various login contexts

---

## Conflict Changes
### CHG-35 – Finalized Backup Strategy Based on Conflict Resolution  
Date: 2025-06-20  
Proposed By: Soukmaed Ong Yu Kang  
Req ID: CF-01  
Session ID: VS-02  
Sections Affected: 3.10.1.3

**What Changed/Added**:  
- Adopted a unified backup policy of daily full backups while maintaining a 30-minute recovery time objective (RTO).  
- Removed conflicting references to other backup intervals.

**Why It Was Changed/Added**:  
- Previous documentation had unclear or conflicting backup frequencies.  
- Resolved the conflict by aligning with the best practice used in § 3.10.1.3.

**Impact**:  
- Ensures the system is backed up consistently and meets recovery requirements.  
- Improves clarity for infrastructure and deployment teams.



### CHG-36 – Finalized Data Retention Policy to Comply with PDPA  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: CF-02  
Session ID: VS-02  
Sections Affected: 1.3.2.1.1, 1.3.2.3, 3.7.9

**What Changed/Added**:  
- Defined exact data retention durations:
  - User data: 2 years after account closure  
  - Academic records: retained indefinitely  
  - Payment records: 7 years  
- Applied across all relevant sections referencing data storage or privacy.

**Why It Was Changed/Added**:  
- There were conflicting retention guidelines between technical, legal, and business needs.  
- This change brings all parts of the document in line with PDPA and institutional requirements.

**Impact**:  
- Ensures legal compliance and accreditation alignment.  
- Clarifies retention for system implementers and auditors.



### CHG-37 – Standardized System Capacity to 5,000 Users  
Date: 2025-06-20  
Proposed By: Tan Jun Xian  
Req ID: CF-03  
Session ID: VS-02  
Sections Affected: 3.5.2, Performance & Testing References

**What Changed/Added**:  
- Reworded Section 3.5.2 to clarify:
  - Normal load: 4,000 users  
  - Peak tested load: 5,000 users  
- Ensured all related specs, tests, and assumptions now reference 5,000 users consistently.

**Why It Was Changed/Added**:  
- Previous sections used inconsistent numbers (e.g., “4,000+” or “5,000”) without explanation.  
- This change resolves the discrepancy and documents load expectations clearly.

**Impact**:  
- Provides a single target for developers, testers, and architects to follow.  
- Eliminates confusion and reduces risk of under-testing.
