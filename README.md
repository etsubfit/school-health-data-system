# school-health-data-system
Designed and implemented a clinical database for 10,000+ school health records. Covers database schema, ETL workflow, and PowerBI dashboards built for stakeholder decision-making. Portfolio piece only—no patient data included.

### From 10,000 paper records to a structured clinical database and stakeholder dashboards.

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
| **Clinical** | Encounter-level medical data | `visits`, `vitals`, `complaints`, `diagnoses`, `management` |
| **Academic** | School & grade context | `schools`, `academic_history`, `school_years` |
| **Nutritional** | Growth monitoring | `anthropometry`, `muac` |
| **Screening** | Population health checks | `screenings`, `screening_types` |
| **Disease Surveillance** | Chronic & allergic conditions | `chronic_illnesses`, `allergies` |

> Full schema documentation: [`docs/database-schema.md`](./docs/database-schema.md)

---

## 🔄 Data Workflow

Paper Records → Standardized Data Entry (Google Sheets) → Cleaning & Validation → Relational Database (SQL) → PowerBI Dashboards → Stakeholder Reports

> Full process documentation: [`docs/data-workflow.md`](./docs/data-workflow.md)

---

## 📊 Sample Dashboard Outputs

Dashboards translated raw data into **stakeholder-ready insights**:

- Vaccination coverage by school and grade
- Nutritional status tracking (BMI-for-age, MUAC)
- Disease prevalence maps across campuses
- Screening completion rates and referral follow-up

> Mock-up examples: [`docs/dashboard-mockups.md`](./docs/dashboard-mockups.md)

---

## 🛠 Tools Used

`SQL` `Excel` `Google Sheets` `PowerBI` `Python` `R` `Clinical Workflow Design`

---

## 👤 Project Lead

**Etsub Fithaamlak, M.D.**
General Practitioner | Clinical Data Specialist
[GitHub Profile Link]
