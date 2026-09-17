# Secure E-Documentation Verification System

A high-integrity e-governance platform designed to eliminate document forgery, unauthorized alterations, and duplicate submissions through automated cryptographic fingerprinting, blockchain-inspired auditing, and instant verification controls.  

## Core Capabilities

* **Cryptographic Fingerprinting:** Generates unique 256-bit SHA-256 hash signatures for every ingested file to ensure permanent data integrity.  
* **Tamper & Duplicate Detection:** Instantly flags tampered files or duplicate submissions by comparing fresh file signatures against stored cryptographic records.  
* **Role-Based Access Control (RBAC):** Enforces strict privilege separation with custom workflows for Admins (issuance), Verifiers (audit & check), and Users (access & download).  
* **Blockchain-Inspired Audit Trail:** Records mock transaction IDs (`0x...`) with server-side timestamps to create an immutable log of document states.  
* **Real-Time Status Tracking:** Automatically classifies every record into clear operational states: Verified, Pending, Duplicate, Rejected, or Tampered.  

## System Architecture & Tech Stack

* **Core Engine:** Python (Flask Micro-framework)  
* **Database & Persistence:** MySQL Relational Database  
* **Security & Cryptography:** SHA-256 Hash Algorithm (`hashlib`)  
* **Presentation Layer:** HTML5, CSS3, JavaScript  
* **Development Environment:** Visual Studio Code, Windows / macOS  

## System Workflow

1. **Document Issuance:** An Admin uploads an official digital file and assigns it to a recipient.  
2. **Hash & Ledger Generation:** The system computes the file's SHA-256 cryptographic signature and registers a unique transaction entry.  
3. **Verification Request:** A Verifier or User submits a file or document token for authenticity validation.  
4. **Automated Integrity Check:** The application recalculates the signature and compares it directly against the database record.  
5. **Verdict & Logging:** The system displays the real-time status (Verified vs. Tampered) and logs the activity in the audit trail.  

## Documentation & Repository Navigation

Click the links below to inspect detailed system views and interface logs:

* [Admin Dashboard Screen](assets/admin_dashboard.png) – Interface for official document issuance and system monitoring.  
* [Verifier Panel View](assets/verifier_dashboard.png) – Inspection panel for tracking verification logs and access histories.  
* [Document Verification Details](assets/document_details.png) – Detailed breakdown of SHA-256 tokens and transaction IDs.  
* [User Portal View](assets/user_dashboard.png) – Client dashboard for accessing and downloading verified documents.  
* 📄 [Download Full System Report (PDF)](assets/project_report.pdf) – Complete technical documentation and performance evaluation report.
