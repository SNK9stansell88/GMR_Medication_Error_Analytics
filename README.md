# Clinical Safety Analytics Pipeline – Medication Error Analysis (GMR)

This repository demonstrates a complete clinical safety analytics workflow built for Global Medical Response (GMR).  
It combines **30 years of clinical insight** with **modern analytics, forecasting, clustering, and machine-learning techniques** to reveal patterns in medication errors and support future AI-driven safety initiatives.

This project is designed for:

- **Jennifer Fletcher**, VP of Clinical Services  
- **John Paul (JP) Feliciano**, Clinical Safety Data Analyst  

---

# 1. Project Overview

This project analyzes medication-error events across all GMR certificates using a structured, multi-notebook analytics pipeline.  
It demonstrates how clinical expertise and analytics work together to uncover safety risks, quantify operational differences, create predictive insights, and support future real-time guidance tools.

---

# 2. Objectives of the Analysis

- Summarize medication-error trends  
- Identify common patterns and medications involved  
- Compare patterns by **Branch (Air/Ground)** and **Certificate**  
- Engineer features to support modeling  
- Cluster error types into meaningful groups  
- Perform inferential tests to validate differences  
- Build a simple decision-tree risk model  
- Forecast future medication-error frequency  
- Integrate results into a leadership-facing narrative  

---

# 3. Dataset Description

**Source:** `Krista_240726_Final.xlsx`  

**Sheets used:**

- **Medication** — event-level details  
- **Med Error Summary** — certificate-level totals  

**Data preparation included:**

- Standardizing Branch and Source labels  
- Cleaning medication and pattern fields  
- Creating clinical pattern flags and medication-group indicators  
- Preparing monthly time-series data  
- Constructing a binary target for risk modeling  

---

# 4. Methods & Notebooks

**01 — Data Overview**  
Basic inspection of columns, missing values, and dataset shape.

**02 — Univariate EDA**  
Distribution of patterns, medications, branch, certificate.

**03 — Bivariate Analysis**  
Cross-tabs of patterns by Branch (Air/Ground) and Certificate.

**04 — Feature Engineering**  
Clinical flags, medication groups, and operational indicators.

**05 — Clustering**  
K-means grouping of medication-error events with similar characteristics.

**06 — Inferential Statistics**  
t-tests (Air vs Ground) and ANOVA (Certificate differences).

**07 — Decision Tree Model**  
Simple, interpretable prediction model for high-risk events.

**08 — Forecasting**  
Holt linear trend model forecasting monthly medication-error counts.

**09 — Integrated Summary**  
Leadership-oriented synthesis of all insights.

---

# 5. Key Findings (High-Level)

- Most common patterns include wrong medication, dose errors, sedation-related issues, documentation errors.  
- Variation exists between **Air and Ground** as well as across certificates.  
- Clustering reveals coherent themes: dose-related, wrong-medication, sedation/analgesia clusters.  
- Inferential testing confirms significant operational differences.  
- Decision tree modeling identifies primary drivers of high-risk events.  
- Forecasting provides forward visibility into medication-error volume.

---

# 6. Clinical & Operational Implications for GMR

- Certificate-level variation highlights opportunities for focused training and protocol reinforcement.  
- Clusters support targeted safety initiatives tailored to operational patterns.  
- Predictive modeling lays groundwork for real-time risk identification and future AI-supported clinical guidance.  
- Forecasting informs staffing, education, and proactive safety planning.

This project demonstrates how clinically grounded analytics can strengthen patient safety across the GMR system.

---

# 7. Repository Structure

```
GMR_Medication_Error_Analytics/
│
├── README.md
├── data/
│     └── Krista_240726_Final.xlsx
│
├── notebooks/
│     ├── 01_data_overview.ipynb
│     ├── 02_univariate_eda.ipynb
│     ├── 03_bivariate_branch_certificate.ipynb
│     ├── 04_feature_engineering.ipynb
│     ├── 05_clustering.ipynb
│     ├── 06_inferential_statistics.ipynb
│     ├── 07_decision_tree_model.ipynb
│     ├── 08_forecasting.ipynb
│     └── 09_integrated_summary.ipynb
│
├── docs/
│     ├── executive_summary.pdf
│     ├── med_error_report.pdf
│     └── clinical_safety_job_description.docx
│
└── results/
      ├── cluster_output.csv
      ├── model_metrics.txt
      ├── forecast_plot.png
      └── feature_table_preview.csv
```

---

# 8. How This Supports Future AI/ML Work at GMR

This project establishes the foundation for:

- Real-time AI patient-care guidance  
- Automated medication-error early-warning systems  
- Predictive dashboards for clinical leaders  
- NLP-based integration with ImageTrend ePCR and device data  
- Safety models aligned with GMR clinical guidelines  

---

# 9. About the Author

- 30 years of clinical and air medical practice  
- Advanced practice provider with broad critical-care background  
- Experienced Base Medical Manager (AeroCare 5)  
- Leader in medication-safety, QA, protocol updates, and operational performance  
- MBA-trained with emphasis on analytics, forecasting, and systems thinking  
- Preparing for Clinical Safety Data Analyst roles aligned with GMR’s future needs  

---

# Attachments Used (GMR Prompt Requirement)

- Med Error 251201 1610.pdf  
- Executive Summary.pdf  
- Krista_240726_Final.xlsx  
- All ML/statistics instructional documents  
- Resume, background files, and job description  
