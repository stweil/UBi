---
title: "Verwaltung von Mitarbeiterfunktionen in eJourney: Empfänger- und Absenderrollen"
source_url_de: (Not provided)
source_url_en: https://www.uni-mannheim.de/en/
category: Benutzung
tags: ['eJourney', 'Mitarbeiter', 'Bewerbung', 'Zuweisung', 'Programm', 'Verwaltung', 'Empfänger', 'Absender']
language: en
---

# Staff Feature Management in eJourney

This guide outlines the specific functionalities available to **Receiving Staff** (host institutions) and **Sending Staff** (home institutions) within the eJourney platform, covering program setup, application monitoring, and data management.

## 🧑‍🏫 Receiving Staff Functions (Host Institution)

Receiving Staff manage the intake and processing of applications for programs hosted by their institution.

### 1. Orientation and Program Setup

Before applications can be managed, the program must be configured:

- **Data Hub Upload:** Program information must first be created and published in the separate **Data Hub**. Receiving Staff are responsible for uploading and maintaining this data.
- **eJourney Configuration:** Once published, the data transfers to eJourney. Staff can access the program via the [ENGAGE.EU Admin menu](https://www.uni-mannheim.de/engageeu-ejourney-online-help/explore-features/managing-staff-features/).
- **Program Settings:** Staff can tailor the application process by configuring key dates and capacities:
  - **Capacity:** Maximum number of admitted students.
  - **Application Start/End Date:** The window for students to submit applications.
  - **Nomination Deadline:** Deadline for sending institutions to nominate students.
  - **Admission Deadline:** Deadline for the host institution to confirm admissions.
  - **Admission Acceptance Deadline:** Deadline for admitted students to accept the offer.

### 2. Application Monitoring

Receiving Staff have access to two key overview features:

#### Application Summary Graph

This visual tool monitors the distribution of applications across partner universities during the application period.

- **Purpose:** Allows staff to monitor application volume and identify universities needing outreach.
- **Note:** The graph only reflects applications currently in the system and counts may decrease after processing by sending institutions. Reviewing it before the nomination phase is recommended.

#### Admission Overview

This provides a consolidated view of all applicants nominated or waitlisted by their home institutions.

- **Availability:** Only visible *after* sending institutions have completed the nomination process.
- **Data Displayed:** For each applicant, the overview shows: Programme ID, Title, Name, Email, European Student Identifier (ESI), Matriculation Number, Birthdate, Gender, Degree, Degree Level, Current Funding, Application Score, and Current Application Status.
- **Filtering:** The **Application Status** field allows filtering by nomination or waitlist status.

### 3. Data Export (Admission Overview)

Receiving Staff can download the **Admission Overview** as an Excel file.

- **Use Case:** Enables offline work, advanced sorting, filtering, or internal sharing of admission offers.
- **Important Limitation:** The downloaded file **does not** include application documents (e.g., transcripts or motivation statements); these are only accessible to Sending Staff.

______________________________________________________________________

## 🧑‍🎓 Sending Staff Functions (Home Institution)

Sending Staff manage the process of selecting and nominating their own students for programs.

### 1. Application Overview

This feature provides a consolidated view of all applicants from the sending institution who have applied to various programs.

- **Purpose:** Supports the nomination process by allowing staff to review and manage applications before submitting final decisions.
- **Data Displayed:** For each applicant, the overview shows: Programme ID, Title, Name, Email, ESI, Matriculation Number, Birthdate, Gender, Degree, Degree Level, Current Funding, Application Score, and Current Application Status.

### 2. Data Export (Application Overview)

Sending Staff can download the full **Application Overview** as a ZIP file for comprehensive offline processing and record keeping.

- **ZIP File Contents:**
  - An Excel file containing all data from the Nomination Overview.
  - Applicant-uploaded documents, including:
    - Motivation Statements
    - Transcripts of Records
- **Folder Structure:** The ZIP file is organized by `Programmes` $\\rightarrow$ `[Programme ID]` $\\rightarrow$ `Applicants` $\\rightarrow$ `[ESI_last name]` $\\rightarrow$ `Documents` (containing the uploaded statements/transcripts).
- **Crucial Step:** Users **must extract** the ZIP file to access the attached documents.
