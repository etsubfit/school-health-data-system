# Data Workflow Documentation

## The Journey: Paper to Decision

This document describes the end-to-end process of transforming paper-based school health records into a structured database and actionable stakeholder reports.

---

## Stage 1: Collection (The Front Line)

**What happened:**

- School clinicians recorded every student encounter on paper health cards and clinic registers
- Data fields included complaints, vitals, physical findings, diagnoses, management, and outcomes
- Records were generated across multiple school campuses, each with its own filing system

**My role as Team Lead:**

- Trained data collection teams on standardized documentation practices
- Set collection protocols to ensure completeness and consistency
- Supervised teams to maintain quality at the point of entry

---

## Stage 2: Digitization and Structuring

**What happened:**

- Raw paper data was manually entered into standardized Google Sheets templates
- Templates mirrored the final database schema to ensure seamless migration
- Dropdown menus and validation rules in Google Sheets reduced entry errors

**Scale:**

- 10,000+ student health records digitized across multiple school campuses

**My role:**

- Designed the Google Sheets templates to match the database schema
- Ensured every field had a destination table before data entry began
- Managed the digitization timeline across campuses

---

## Stage 3: Cleaning and Validation

**What happened:**

- Duplicate records identified and resolved
- Missing values flagged and addressed (required fields enforced at entry)
- Outlier detection on continuous variables (vitals, anthropometry, RBS)
- Cross-validation: student counts reconciled against school enrollment registers
- Referential integrity checks: every visit linked to a valid student, school, and clinician

**My role:**

- Performed data cleaning using Excel, Google Sheets, and SQL queries
- Built validation rules to catch errors early
- Documented cleaning decisions for transparency and reproducibility

---

## Stage 4: Automated Database Creation and Load

**What happened:**

- Wrote a Python script that created the full database schema programmatically (TemariCare)
- Used the Google Sheets API to read data directly from structured sheets
- The same Python script transformed sheet data into relational format and loaded it into the database
- Referential integrity enforced programmatically during the load process
- Indexes created on frequently queried columns for performance

**Verification:**

- Used MySQL Workbench to cross-check the validity of fetched data
- Ran spot-check queries to confirm row counts matched source sheets
- Verified key relationships (every visit had a valid student, school, and clinician)

**Why automation mattered:**

- Eliminated manual CSV exports and imports
- Allowed incremental updates as new records were digitized
- Reduced human error in the migration step
- Made the pipeline reproducible and auditable

**My role:**

- Designed the database schema before any code was written
- Wrote the Python script for schema creation and data loading
- Used MySQL Workbench for data validation and integrity checks
- Tested and debugged the pipeline until it ran reliably

---

## Stage 5: Analysis and Visualization

**What happened:**

- SQL queries aggregated data into key health indicators
- PowerBI dashboards built with stakeholder-appropriate views
- Five dashboard categories created:
  1. Clinical Operations Overview
  2. Morbidity Surveillance
  3. Clinical Decision-Making Analysis
  4. Student Health and Screening
  5. Patient Outcomes

**My role:**

- Wrote all core aggregation queries
- Designed dashboard layouts for clarity and actionability
- Prepared PowerPoint summaries for non-technical stakeholders

---

## Stage 6: Action (The Outcome)

**What happened:**

- Stakeholders used reports to allocate resources (e.g., targeted deworming campaigns)
- Schools with low screening coverage were identified for follow-up
- High medication rejection rates in specific campuses triggered health education interventions
- Data-driven decisions replaced anecdotal reporting

**My role:**

- Presented findings to program managers and school health coordinators
- Translated dashboard insights into plain-language recommendations
- Established a reporting cadence (monthly/quarterly) for sustained impact

---

## Technical Summary

Paper Records → Standardized Data Entry (Google Sheets) → Cleaning and Validation (Python, SQL) → Automated Schema Creation and ETL via Python (Google Sheets API to MySQL) → Data Verification (MySQL Workbench) → PowerBI Dashboards (5 suites) → Stakeholder Reports and Action

**Key tools:** Python, Google Sheets API, MySQL, MySQL Workbench, SQL, PowerBI, Excel

---

## Why This Workflow Matters

This was not a theoretical exercise. It was a real implementation in a resource-constrained setting. The automated pipeline meant the entire process, from schema creation to data loading, ran through a single Python script. MySQL Workbench served as the verification layer, ensuring the automation worked correctly before dashboards were built on top.

Every stage, from training collectors to writing the ETL script to presenting dashboards, was designed to answer one question:

*Are our students healthy, and if not, what are we doing about it?*

The data workflow made that question answerable for the first time.
