# Dashboard Mock-ups

Actual patient data has been redacted. The following describes the four dashboard tabs built in PowerBI, including all visuals, filters, and cards.

---

## Tab 1: Visits, Outcomes and Management

**What it covers:** Clinical utilization, patient outcomes, and management patterns across campuses.

**Visuals:**

| Visual | Type | Purpose |
|:---|:---|:---|
| Visit trends over time | Line chart | Track clinical demand weekly/monthly |
| Total visits per campus | Bar chart | Compare utilization across schools |
| Total clinical visits per student | Table | Identify high-utilization students |
| Outcome distribution | Pie chart | Returned to class vs. sent home vs. referred |
| Management category distribution | Donut chart | Conservative, counseling, medication, procedural |
| Management categories by campus | Clustered column chart | Compare management patterns across schools |

**Filters:** Gender, school, grade

**Cards:** Total visits, total students who had clinical visits

**Why it mattered:**
This tab gave program managers a single view of clinical demand, patient flow, and management behavior. The clustered column chart revealed whether certain campuses relied more heavily on medication versus conservative management. The outcomes pie chart showed whether students were being sent home at disproportionate rates.

---

## Tab 2: Complaints and Diagnoses

**What it covers:** Morbidity surveillance and syndromic tracking.

**Visuals:**

| Visual | Type | Purpose |
|:---|:---|:---|
| Complaint counts | Bar chart | Top presenting complaints ranked |
| Diagnosis counts | Bar chart | Most common diagnoses ranked |
| Complaint word cloud | Word cloud | Quick visual summary of frequent complaints |

**Filters:** School, gender, grade

**Cards:** Total students for clinical visits

**Why it mattered:**
The bar charts enabled ranked comparison of disease burden. The word cloud gave a rapid, intuitive snapshot of dominant complaints—useful for non-clinical stakeholders. Filtering by school allowed instant comparison of morbidity profiles across campuses.

---

## Tab 3: Top 5 Management Types per Category

**What it covers:** Clinical decision-making granularity—what exactly did clinicians do within each management category?

**Visuals:**

| Visual | Type | Purpose |
|:---|:---|:---|
| Top 5 conservative management types | Bar chart | Most common conservative treatments |
| Top 5 counseling and education types | Bar chart | Most common health education topics |
| Top 5 medication types | Bar chart | Most prescribed medications |
| Top 5 procedural types | Bar chart | Most performed procedures |

**Cards:** Medication rejection rate, recommendation rate, referral rate

**Why it mattered:**
This tab moved beyond "what category" to "what specifically." It revealed whether prescribing patterns were appropriate, whether counseling was being utilized, and whether high rejection or referral rates in specific campuses needed investigation.

---

## Tab 4: Nutritional Assessment

**What it covers:** Growth monitoring, malnutrition screening, and diabetic student tracking.

**Visuals:**

| Visual | Type | Purpose |
|:---|:---|:---|
| BMI category distribution | Pie chart | Normal weight, underweight, overweight, obese |
| BMI categories by campus | Bar chart | Compare nutritional status across schools |
| BMI vs. age | Scatter plot | Identify age-based growth patterns and outliers |
| RBS monitoring | Line chart | Blood sugar trends per diabetic student |
| MUAC monitoring | Line chart | Mid-upper arm circumference with SAM/MAM thresholds |
| Height vs. weight | Scatter plot | Visualize growth distribution with BMI color coding |

**Filters:** School, gender, grade

**Cards:** Student count for clinical visits

**Why it mattered:**
Nutritional status is a leading indicator of child health. The dual scatter plots (BMI vs. age and height vs. weight) gave two complementary views of growth. RBS and MUAC trend lines enabled individualized monitoring of diabetic and malnourished students. Filtering by school revealed which campuses needed urgent nutritional interventions.

---

## Summary

| Tab | Primary Question Answered |
|:---|:---|
| Visits, Outcomes and Management | Who came, what happened to them, and how were they managed? |
| Complaints and Diagnoses | What are students presenting with and being diagnosed with? |
| Top 5 Management Types | What specifically did clinicians do within each management category? |
| Nutritional Assessment | Are students growing properly and where are the nutritional risks? |

---

## Note

Screenshots are excluded to protect patient data. Demo versions can be recreated using PowerBI's sample datasets upon request.
