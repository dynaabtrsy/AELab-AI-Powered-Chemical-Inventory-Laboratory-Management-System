# AELab | AI-Powered Chemical Inventory & Laboratory Management System

AELab is a digital laboratory management platform designed to centralise chemical inventory, requests, approvals and activity tracking. Built using Google AppSheet, Google Apps Script and Google Workspace, the system integrates Gemini AI to generate usage insights, support replenishment planning and provide chemical safety assistance.

The platform aims to improve laboratory operations through automated workflows, structured inventory records and inclusive user interface design that reduces cognitive load for laboratory personnel.

---

## Table of Contents

1. [Overview](#-1-overview)
2. [Executive Summary](#-2-executive-summary)
3. [Methodology](#%EF%B8%8F-3-methodology)
4. [Key Findings](#-4-key-findings)
5. [Recommendations](#-5-recommendations)
6. [Limitations](#%EF%B8%8F-6-limitations)
7. [Project Impact](#-7-project-impact)
8. [Apps Overview & Demo Video](#-8-apps-overview--demo-video)
9. [Technologies & Tools](#%EF%B8%8F-9-technologies--tools)

---

## 🔍 1. Overview

### Background

Chemical laboratories manage a wide range of chemicals that require consistent monitoring, accurate inventory records and proper safety documentation.

However, existing laboratory practices often rely on separate spreadsheets, paper request forms, emails and physical logbooks. This creates fragmented information, making it difficult for laboratory personnel to monitor stock levels, retrieve transaction histories and identify chemicals approaching their expiry dates.

AELab was proposed to address these operational challenges by connecting the chemical inventory lifecycle through a single digital platform.

### Problem Statement

Based on interviews with three Science Officers at IIUM Kuantan, several operational challenges were identified:

| Identified Challenge | Reported Situation |
|---|---:|
| Chemicals managed | 516 chemicals |
| Chemical requests | Approximately 500 per semester |
| Inventory discrepancies | 60% of records differed from physical counts |
| Late stock and expiry detection | Approximately 99% |
| Missing Safety Data Sheets (SDS) | Almost 98% of chemicals checked |

These findings highlighted the need for a centralised system that improves inventory visibility, transaction traceability and proactive monitoring.

### Proposed Solution

AELab introduces an integrated application that connects six key operational areas:

- **Chemical Catalogue:** Centralised chemical records with stock status, storage location and expiry information.
- **Request & Approval:** Digital chemical request submissions, approval workflows and status tracking.
- **Activity Log:** Time-stamped records of chemical requests, stock additions and stock deductions.
- **Expiry & Low Stock Alerts:** Automated notifications for chemicals approaching expiry or falling below minimum stock levels.
- **Monthly Usage & Prediction Report:** Gemini AI-assisted analysis of consumption patterns and replenishment requirements.
- **Audit Dashboard:** Inventory monitoring and visibility into frequently used and near-expiry chemicals.

Additional features include OCR-based chemical searching, voice-assisted chemical location and Gemini-powered chemical safety assistance.

---

## 📊 2. Executive Summary

AELab transforms fragmented laboratory inventory processes into a connected digital workflow.

The application combines AppSheet for operational management, Google Sheets for centralised data storage, Google Workspace for automation and Gemini AI for analytical support.

### Project Objectives

1. Centralise chemical inventory records and standardise data management.
2. Digitise chemical request submissions and approval processes.
3. Improve stock visibility through automated monitoring and alerts.
4. Maintain a traceable history of chemical movements and user activities.
5. Apply AI-assisted insights to support inventory replenishment planning.
6. Improve accessibility through simplified navigation, clear instructions and voice-assisted features.

### System Architecture

The platform follows a connected workflow:

| Component | Function |
|---|---|
| Google Sheets | Centralised database and inventory records |
| AppSheet | Application interface and operational workflows |
| Google Apps Script | Workflow automation and integrations |
| Gmail | Automated request confirmations and alerts |
| Google Calendar & Tasks | Replenishment reminders |
| Gemini AI | Monthly usage analysis and safety assistance |
| Looker Studio | Dashboard and analytical visualisation |

### User Roles

**General Users – Lecturers and Science Officers**
- Search and view chemical information.
- Submit chemical requests.
- Track request status.
- Receive automated email notifications.

**Administrators – Laboratory PICs and Store PICs**
- Review, approve or reject requests.
- Record stock additions and deductions.
- Monitor chemical inventory and expiry dates.
- Review activity records and audit dashboards.
- Receive monthly usage and prediction reports.

---

## ⚙️ 3. Methodology

The project followed a problem-identification, system-design, development and preliminary-testing approach.

### 3.1 Requirements Gathering & Problem Identification

Three Science Officers were interviewed to understand existing laboratory inventory practices and operational difficulties.

The findings were used to identify requirements involving:
- Chemical catalogue management.
- Inventory accuracy and stock monitoring.
- Request submission and approval.
- Expiry tracking and safety documentation.
- Transaction traceability.
- Automated reporting and replenishment planning.

### 3.2 Data Management & System Design

A structured database was designed using Google Sheets, with interconnected tables to manage different operational records.

| Database Table | Purpose |
|---|---|
| Chemical List | Stores chemical details, CAS numbers, hazards and storage information |
| Inventory | Records stock quantities, expiry dates and inventory transactions |
| Requests | Stores request details, quantities and approval statuses |
| Activity Log | Maintains records of user activities and chemical movements |
| Access | Defines user information and role-based permissions |

Unique identifiers, such as Chemical ID and Request ID, connect related records to maintain traceability.

### 3.3 Application Development & Workflow Automation

The application was developed using Google AppSheet and integrated with Google Workspace tools.

Key development components included:

- Interactive chemical catalogue and inventory views.
- Digital request and approval forms.
- Role-based access management.
- Automated email notifications.
- Time-stamped activity logging.
- Low-stock and near-expiry alerts.
- Voice-assisted chemical search.
- OCR-based chemical identification.

### 3.4 AI Integration

Gemini AI was integrated to support two main functions:

**Monthly Usage & Prediction Report**
- Analyse historical chemical consumption records.
- Summarise monthly inventory usage.
- Identify consumption patterns and potential anomalies.
- Provide replenishment suggestions for administrator review.

**Chemical Safety Assistance**
- Generate chemical-specific safety summaries.
- Provide hazard information and relevant SDS references.
- Offer bilingual assistance in Bahasa Melayu and English.
- Support users with preliminary, step-by-step safety guidance.

AI-generated outputs are intended to support administrative decisions and must be reviewed by appropriate personnel.

### 3.5 Dashboard & UI Design

The dashboard and application interface were designed to provide a clear overview of laboratory inventory conditions.

The design focused on:
- Clear navigation between application modules.
- Visual identification of low-stock and near-expiry chemicals.
- Simplified forms and structured information.
- Consistent layouts and status indicators.
- Reduced cognitive load through clear instructions and reminders.

### 3.6 Preliminary Testing

Initial testing involved two users and two administrators to assess basic application functionality.

| Test Area | Preliminary Observation |
|---|---|
| Chemical request submission | Completed in under 1 minute |
| Confirmation email | Received within 10 seconds |
| Request status updates | Automated notifications triggered upon status changes |
| Stock and expiry alerts | Triggered during initial tests |
| Voice search | Matched spoken chemical names in 80% of tests |

The monthly automation schedule was simulated during early testing. A larger pilot involving 40 users over one semester was proposed for further evaluation.

---

## 📈 4. Key Findings

### 4.1 Operational Challenges

The interviews highlighted several weaknesses in the existing inventory management process:

- **Fragmented records:** Chemical information was distributed across spreadsheets, forms and physical logbooks.
- **Inventory discrepancies:** Recorded stock quantities did not always match physical inventory.
- **Manual monitoring:** Expiry dates and stock levels depended heavily on manual checking.
- **Limited traceability:** Retrieving historical chemical transactions required reviewing physical records.
- **Incomplete safety documentation:** Many of the chemicals checked did not have readily available SDS documentation.

### 4.2 Preliminary Application Testing

Initial testing demonstrated the potential of digital workflows to reduce administrative effort.

Three notable observations were:

1. Chemical requests could be submitted in under one minute.
2. Confirmation emails were delivered within 10 seconds during initial tests.
3. Voice search achieved an 80% matching rate during preliminary testing.

These observations provide early evidence of application functionality, rather than conclusive results from a full laboratory deployment.

### 4.3 Key Takeaway

AELab demonstrates how centralised records, workflow automation and AI-assisted analysis can work together to improve inventory visibility and support more proactive laboratory management.

---

## 💡 5. Recommendations

Based on the identified operational challenges and preliminary testing, the following improvements are recommended.

| Area | Recommendation | Expected Benefit |
|---|---|---|
| Data Management | Standardise chemical records and enforce mandatory fields | Improve data consistency and inventory accuracy |
| Inventory Monitoring | Introduce automated stock reconciliation | Reduce discrepancies between recorded and physical stock |
| Workflow Automation | Expand automated request and approval notifications | Reduce manual follow-ups |
| Expiry Management | Implement scheduled expiry monitoring | Support earlier identification of chemicals requiring action |
| Predictive Analytics | Evaluate historical consumption patterns and forecast accuracy | Improve replenishment planning |
| AI Integration | Introduce human review for AI-generated outputs | Reduce risks associated with inaccurate recommendations |
| User Experience | Conduct usability testing with different user groups | Improve accessibility and ease of use |
| Scalability | Extend the system to other laboratory departments | Establish a consistent inventory management framework |

---

## ⚠️ 6. Limitations

Despite its potential, several limitations should be considered.

**1. Limited Testing Population**

Initial testing involved only two users and two administrators. The results may not represent the experience of the wider laboratory population.

**2. Prototype Validation**

The system was developed as a prototype. A full-scale deployment and longer-term operational evaluation are still required.

**3. AI Prediction Reliability**

Gemini-generated replenishment insights depend on the quality and completeness of historical inventory records. AI-generated recommendations should remain advisory and require administrator validation.

**4. Voice Recognition Accuracy**

Preliminary voice search achieved an 80% matching rate. Performance may vary depending on pronunciation, background noise and chemical naming conventions.

**5. Data Quality and Synchronisation**

Inconsistent data entry, missing fields and synchronisation delays may affect inventory accuracy and automated alerts.

**6. Integration Dependencies**

The system relies on Google Workspace, AppSheet and external AI services. Application functionality may be affected by platform availability, permissions and service limitations.

---

## 🚀 7. Project Impact

AELab aims to improve laboratory operations by connecting inventory management, request processing, transaction tracking and AI-assisted planning.

### Expected Operational Improvements

| Operational Area | Proposed Target |
|---|---|
| Chemical request submission | 10 minutes → 1 minute |
| Request approval interaction | 3 days → 5 seconds |
| Request status retrieval | 3 days → 1 second |
| New laboratory setup | Within 1 day |
| Expired stock identification | 6 months → 1 month |

*Note: These are proposal targets, not fully validated performance improvements. Early testing demonstrated request completion in under one minute and confirmation emails within 10 seconds.*

### Stakeholder Benefits

- **Laboratory Personnel:** Easier chemical searches, request submissions and status tracking.
- **Laboratory Administrators:** Improved inventory monitoring, traceable records and automated alerts.
- **Institution:** A more standardised approach to chemical inventory management and documentation.
- **Other Laboratories:** Potential to replicate the system through structured data imports and configurable workflows.

### Institutional Alignment

The project supports:
- MOHE Dasar Pendigitalan Pendidikan Tinggi 2025–2030.
- Occupational Safety and Health Act 1994 (Act 514).
- USECHH Regulations 2000.
- United Nations Sustainable Development Goal 10: Reduced Inequalities, through inclusive design considerations.

---

## 📱 8. Apps Overview & Demo Video

AELab consists of interconnected modules designed to support different stages of chemical inventory management.

### 8.1 Application Dashboard

![AELab Dashboard](https://github.com/user-attachments/assets/d2f252d3-ebe7-455c-8abd-a2a16d46f6cb)


Provides an overview of laboratory inventory conditions, including stock health, low-stock items and near-expiry chemicals.

### 8.2 Chemical Inventory Catalogue

![Chemical Inventory](https://github.com/user-attachments/assets/17c2eab8-ef38-4eab-9782-c580be1aa0e2)

Allows users to search and view chemical information, stock availability, physical form and storage details.

### 8.3 Request & Approval 

<img width="200" height="400" src="https://github.com/user-attachments/assets/9cfb5745-8511-40ad-b622-5ec6ed00e572" />

<img width="200" height="400" src="https://github.com/user-attachments/assets/c0637122-dfdb-487d-a94f-f4f82b109588" />


Digitises chemical request submissions and approval processes, with automated status notifications.

### 8.4 Activity Log

![Activity Log](https://github.com/user-attachments/assets/0b100a7e-c941-4581-9f82-7e759d0a0c6c)

Maintains a time-stamped record of chemical requests, stock additions and deductions for improved traceability.

### 8.5 Gemini AI Integration

Gemini AI Safety Bot & AI Chatbot:

<img width="200" height="400" src="https://github.com/user-attachments/assets/054381d1-e01e-4284-90c2-d1a9de8cc227" />



Automated Email Alert:

![Email Alert](https://github.com/user-attachments/assets/a7c8e668-2384-4562-8880-f2bee86481c9)


Provides AI-assisted chemical safety information, bilingual guidance and monthly inventory usage insights.

### 8.6 Demo Video

**Application Walkthrough:** [Click here to watch a 3-minutes AELab Demo Video Link](https://drive.google.com/file/d/1MMxLv1HJsIC6z8qfeAcCGiDYO9uJbylT/view?usp=sharing)

The demonstration covers:
1. Navigating the AELab dashboard.
2. Searching and locating chemicals.
3. Submitting and approving chemical requests.
4. Monitoring inventory activities.
5. Receiving automated stock and expiry alerts.
6. Exploring Gemini AI features.

---

## 🛠️ 9. Technologies & Tools

| Category | Technologies |
|---|---|
| Application Development | Google AppSheet |
| Database Management | Google Sheets |
| Workflow Automation | Google Apps Script |
| Artificial Intelligence | Google Gemini API |
| Business Intelligence | Looker Studio |
| Communication & Notifications | Gmail |
| Scheduling & Reminders | Google Calendar, Google Tasks |
| UI/UX Design | AppSheet Interface Design |


---

<p align="center">
  <b>AELab | A Smarter, More Connected Approach to Laboratory Management</b><br>
  MOHE Gemini × AppSheet Hackathon 2026
</p>
