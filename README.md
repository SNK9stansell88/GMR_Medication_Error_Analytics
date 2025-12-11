Clinical Safety Analytics Pipeline – Medication Error Analysis (GMR)

This repository demonstrates a complete clinical safety analytics workflow built for Global Medical Response (GMR).
It combines 30 years of clinical insight with modern analytics, forecasting, clustering, and machine-learning techniques to reveal patterns in medication errors and support future AI-driven safety initiatives.

This project is designed for:

Jennifer Fletcher, VP of Clinical Services

John Paul (JP) Feliciano, Clinical Safety Data Analyst

1. Project Overview

This project analyzes medication-error events across all GMR certificates using a structured, multi-notebook pipeline.
It demonstrates how clinical expertise and analytics can work together to uncover safety risks, quantify differences across operations, create predictive insights, and support future real-time guidance tools.

2. Objectives of the Analysis

Summarize medication-error trends

Identify common patterns and medications involved

Compare patterns by Branch (Air/Ground) and Certificate

Engineer features to support modeling

Cluster error types into meaningful groups

Perform inferential testing to validate differences

Build a simple decision-tree risk model

Forecast future medication-error frequency

Integrate results into a leadership-facing narrative

3. Dataset Description

Source: Krista_240726_Final.xlsx
Sheets used:

Medication — event-level details

Med Error Summary — certificate-level totals

Data preparation included:

Standardizing Branch and Source fields

Cleaning medication and pattern fields

Creating clinical pattern flags and medication-group indicators

Preparing monthly time-series data

Constructing a binary target for risk modeling

4. Methods & Notebooks

Each notebook covers one stage in the analytics pipeline:

01 — Data Overview
Basic inspection of columns, missing values, and dataset shape.

02 — Univariate EDA
Frequency and distribution of key fields (patterns, medications, branch, certificate).

03 — Bivariate Analysis
Cross-tab exploration of patterns by Branch (Air/Ground) and Certificate.

04 — Feature Engineering
Creation of domain-specific clinical flags, medication groupings, and operational indicators.

05 — Clustering
K-means clustering to group medication-error events with similar characteristics.

06 — Inferential Statistics
t-tests (Air vs Ground) and ANOVA (Certificate-level differences) to determine which differences are statistically meaningful.

07 — Decision Tree Model
Simple, interpretable model predicting high-risk events using engineered features.

08 — Forecasting
Holt linear trend model predicting future monthly medication-error counts.

09 — Integrated Summary
Final leadership-facing synthesis that integrates the full pipeline and highlights actionable insights.

5. Key Findings (High-Level)

Common patterns include wrong medication, dose errors, sedation-related issues, and documentation inconsistencies.

Operational variation exists between Air and Ground operations and across business units.

Clusters reveal thematic groupings of errors (dose, wrong-medication, sedation/analgesia-related).

Inferential statistics identify statistically significant differences between operational groups.

Decision-tree modeling highlights the strongest predictors of high-risk events.

Forecasting provides early visibility into anticipated medication-error volume.

These insights build a foundation for targeted intervention and system-wide safety improvement.

6. Clinical & Operational Implications for GMR

Variation across certificates signals opportunities for targeted training and protocol reinforcement.

Clusters support focused clinical-safety initiatives aligned with operational patterns.

Predictive modeling establishes a path toward real-time risk identification, aligned with future AI-supported clinical guidance.

Forecasting informs staffing, education, and medication-safety planning at a system-wide level.

This project shows how clinically grounded analytics can support safer, more consistent patient care across the GMR system.

7. Repository Structure
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

8. How This Supports Future AI/ML Work at GMR

This project establishes the analytical foundation for:

Real-time AI patient-care guidance

Automated medication-error early-warning systems

Predictive dashboards for safety officers

NLP-based integration with ImageTrend ePCR and device data

Safety models aligned with GMR clinical guidelines

Together, these steps align with GMR’s long-term vision for data-driven clinical excellence.

9. About the Author

30 years of clinical and air medical practice

Advanced practice provider with broad critical-care experience

Experienced Base Medical Manager (AeroCare 5)

Leader in medication-safety initiatives, QA, protocol education, and operational improvements

MBA-trained with emphasis on analytics, forecasting, and systems thinking

Preparing for Clinical Safety Data Analyst roles aligned with GMR’s strategic quality initiatives

Attachments Used (GMR Prompt Requirement)

Med Error 251201 1610.pdf

Executive Summary.pdf

Krista_240726_Final.xlsx

All ML/statistics instructional documents

Resume, background files, and job description
