# Power-BI-Portfolio

A curated collection of enterprise-grade Power BI analytics solutions demonstrating end-to-end data modeling, DAX engineering, UI/UX dashboard design, and business domain insights.

---

## 🏥 01. Healthcare Operational & Revenue Optimization

An end-to-end clinical and financial analytics platform built to monitor hospital bed capacity, emergency department triage performance, 30-day readmission risk, and revenue realization bottlenecks across clinical specialties.

### 📁 Quick Project Links

* 📂 [Dataset Directory](01_Healthcare%20Analytics/dataset) — *Relational CSV datasets powering the data model.*
* 📂 [Architecture & Schema Specs](01_Healthcare%20Analytics/Architecture%20%26%20Schema) — *Model design documentation and calculations.*
  * 📄 [Core DAX Measures](01_Healthcare%20Analytics/Architecture%20%26%20Schema/Core%20DAX%20Measures) — *Calculated measures for KPIs, financial exposure, and satisfaction indexes.*
  * 📄 [Dashboard Pages and Visuals](01_Healthcare%20Analytics/Architecture%20%26%20Schema/Dashboard%20Pages%20and%20Visuals) — *Detailed page-by-page visual breakdown and key insights.*
* 🖼️ [Screenshots Gallery](01_Healthcare%20Analytics/Screenshots) — *High-resolution dashboard previews.*

---

### 📐 Data Model Architecture

The data model follows a Star Schema architecture, enforcing 1-to-many single-direction relationships between dimension tables and the central `Fact_Visits` table.

![Model Schema](01_Healthcare%20Analytics/Screenshots/Model%20Schema.png)

---

### 📊 Dashboard Visual Walkthrough

#### 1. Care Delivery & Operational Efficiency
Focuses on inpatient length of stay (LOS), bed days, emergency encounter volume, and physician-level treatment vs. medication costs.

![Care Delivery & Operational Efficiency](01_Healthcare%20Analytics/Screenshots/Care%20Delivery%20%26%20Operational%20Efficiency.png)

* **Key KPIs:** Average Length of Stay (4.87 Days), Total Bed Days (1,245), Emergency Visits (1,929), Average Treatment Cost ($526.08), Clinical Overhead ($109.21).
* **Key Visuals:** Revenue & Volume by Service Type, Revenue by Procedure, Average Treatment & Medication Cost by Specialty, and Doctor Operational Performance Matrix.

---

#### 2. Revenue & Financial Overview
Monitors total gross revenue generation, accounts receivable (A/R) exposure, uncollected billing percentages, and payer performance.

![Financial Overview](01_Healthcare%20Analytics/Screenshots/Financial%20Overview.png)

* **Key KPIs:** Gross Revenue ($3M), Total Visits (5,000), Pending Revenue ($1.31M), Uncollected A/R Exposure (39.11%), Average CSAT (3.84/10).
* **Key Visuals:** Monthly Gross Revenue vs. Pending Collection Risk trend chart and Pending A/R Exposure by Insurance Provider bar chart.

---

#### 3. Patient Satisfaction & Quality Index
Evaluates patient experience scores across service settings (Inpatient, Outpatient, Emergency), clinical specialties, and attending physicians.

![Patient Analysis and Bottlenecks](01_Healthcare%20Analytics/Screenshots/Patient%20Analysis%20and%20Bottlenecks.png)

* **Key KPIs:** Average Patient Satisfaction (3.84), 5+ Rating Share (1,766), Low-Rating Risk Share (1,929), Inpatient CSAT (4.37), Outpatient CSAT (3.36).
* **Key Visuals:** Satisfaction breakdown by Specialty, Satisfaction by Service Type, and Provider CSAT Performance Scorecard.

---

## 🛠 Repository Structure

```text
Power-BI-Portfolio/
│
├── 01_Healthcare Analytics/
│   ├── Architecture & Schema/
│   │   ├── Core DAX Measures
│   │   └── Dashboard Pages and Visuals
│   ├── Screenshots/
│   │   ├── Model Schema.png
│   │   ├── Care Delivery & Operational Efficiency.png
│   │   ├── Financial Overview.png
│   │   └── Patient Analysis and Bottlenecks.png
│   └── dataset/
│       ├── Fact_visits.csv
│       ├── Dim_patients.csv
│       └── ...
│
├── LICENSE
└── README.md
