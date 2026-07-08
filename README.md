# School Health Data System

### From 10,000+ paper records to a structured clinical database and stakeholder dashboards.

---

## 📌 Overview

This repository documents my work designing and implementing a comprehensive clinical database for school-based health services. It is a portfolio piece showcasing **clinical data modeling, database design, and health intelligence reporting**—built from real-world experience.

> ⚠️ All patient data has been redacted. This repository demonstrates process, architecture, and outcomes only.

---

## 🎯 The Problem

School health services across multiple campuses relied entirely on **paper-based records**—individual student health cards, handwritten clinic logs, and fragmented registers. There was no way to:

- Track health trends across schools
- Identify outbreaks or clusters early
- Report actionable insights to education and health stakeholders

---

## 🏗️ The Solution: Database Architecture

I designed a relational database organized into **6 core modules**:

| Module | Purpose | Example Tables |
|:---|:---|:---|
| **Student Demographics** | Core identity records | `students`, `genders`, `blood_types` |
| **Clinical** | Encounter-level medical data | `visits`, `vitals`, `complaints`, `diagnoses`, `management`, `outcomes` |
| **Academic** | School & grade context | `schools`, `academic_history`, `school_years` |
| **Nutritional** | Growth monitoring | `anthropometry`, `muac` |
| **Screening** | Student-wide health checks | `screenings`, `screening_types` |
| **Disease Surveillance** | Chronic & allergic conditions | `chronic_illnesses`, `allergies` |

> Full schema documentation: [`docs/database-schema.md`](./docs/database-schema.md)

---

## 🔄 Data Workflow

Paper Records → Standardized Data Entry (Google Sheets) → Cleaning and Validation (Python, SQL) → Automated ETL: Google Sheets API to MySQL via Python (TemariCare) → Data Verification (MySQL Workbench) → PowerBI Dashboards → Stakeholder Reports

> Full process documentation: [`docs/data-workflow.md`](./docs/data-workflow.md)

---

## 📊 Dashboard Suite

Four PowerBI dashboard tabs translated raw clinical data into actionable insights:

| Tab | Key Visuals | Filters |
|:---|:---|:---|
| **Visits, Outcomes and Management** | Visit trends (line), visits per campus (bar), visits per student (table), outcomes (pie), management categories (pie), management by campus (clustered column) | Gender, school, grade |
| **Complaints and Diagnoses** | Complaint counts (bar), diagnosis counts (bar), complaint word cloud | School, gender, grade |
| **Top 5 Management Types** | Top 5 per management category, with rejection rate, recommendation rate, and referral rate (cards) | — |
| **Nutritional Assessment** | BMI categories (pie and bar), BMI vs. age (scatter), RBS monitoring (line), MUAC monitoring (line), height vs. weight (scatter) | School, gender, grade |

> Full dashboard documentation: [`docs/dashboard-mockups.md`](./docs/dashboard-mockups.md)

---

## 🛠 Tools Used

`Python` `Google Sheets API` `MySQL` `MySQL Workbench` `SQL` `PowerBI` `Excel` `R` `Clinical Workflow Design`

---

## 👤 Project Lead

**Etsub Fithaamlak, M.D.**
General Practitioner | Clinical Data Specialist
[github.com/etsubfit](https://github.com/etsubfit)
