# Patient-Profile-Diagnosis-Trends

This project analyzes patient visit data for a healthcare clinic and presents key insights through an interactive Power BI dashboard. The goal is to understand patient demographics, visit utilization patterns, diagnoses, and procedures to support data-driven clinical and operational decision-making.

---

## 📊 Project Overview

The dashboard provides a consolidated view of:
- Patient population demographics
- Visit utilization and high utilizers
- Most frequent diagnoses (ICD codes)
- Most common procedures (CPT codes)
- Time-based trends using visit year filters

The project simulates a real-world healthcare analytics scenario where raw data is transformed into actionable insights for stakeholders.

---

## ❓ Business Questions Answered

- What does the clinic’s patient population look like by age?
- What are the top diagnoses overall?
- How many visits does the average patient have, and who are the high utilizers?
- Which CPT codes (procedures) are performed most often?

---

## 📁 Dataset

- **Source:** `patient_visits.csv`
- **Key fields:**
  - `patient_id`
  - `visit_date`
  - `date_of_birth`
  - `patient_sex`
  - `icd_code`
  - `cpt_code`

The dataset represents patient visits, diagnoses, and procedures over multiple years.

---

## 🔧 Data Preparation & Modeling

Data transformation was performed using **Power Query**:

- Converted text-based date fields into standardized date formats.
- Calculated patient age from date of birth.
- Created age bands:
  - 0–17
  - 18–39
  - 40–64
  - 65+
- Modeled patient-level visit counts to support utilization analysis.
- Identified high utilizers as patients with **4 or more visits**.

---

## 📈 Dashboard Features

### 🔹 Key KPIs
- Total Patients
- Total Visits
- Average Visits per Patient
- High Utilizers (4+ visits)

### 🔹 Visualizations
- Patient distribution by age group
- Patient distribution by sex
- Top 10 diagnoses by visit count (ICD codes)
- Top 10 procedures by frequency (CPT codes)
- Table of high utilizers with visit counts

### 🔹 Interactivity
- Dynamic slicers for:
  - Visit year
  - Sex
  - Age band

All visuals update dynamically based on selected filters.

---

## 📌 Key Insights

- The clinic served **42 unique patients** with **200 total visits**, averaging **4.76 visits per patient**.
- The **40–64 age group** represents the largest portion of the patient population.
- Female patients account for a slightly higher share of visits compared to male patients.
- A small number of diagnoses, led by **hypertension (ICD I10)**, drive a significant portion of visit volume.
- Procedure activity is concentrated among common outpatient evaluation and management CPT codes.
- A subset of high utilizers contributes disproportionately to total visits, indicating opportunities for targeted care management.

---

## 🛠️ Tech Stack

- **Power BI**
  - Power Query
  - DAX
- **Excel**
- **SQL** (conceptual data modeling)

---


## 📬 Contact

If you have questions or feedback about this project, feel free to reach out via LinkedIn or GitHub.
