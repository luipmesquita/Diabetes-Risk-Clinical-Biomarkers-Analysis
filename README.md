# Diabetes-Risk-Clinical-Biomarkers-Analysis

## 📌 Executive Summary

Diagnosing diabetes and assessing metabolic risk strictly through single blood parameters can lead to false positives or missed diagnoses. This project explores the interplay between **Fasting Stabilized Glucose (`stab_glu`)**, **Glycated Hemoglobin (`glyhb`)** (also knowned as HbA1c), and key anthropometric/demographic attributes (**Waist Circumference** and **Age**). 

The goal is to evaluate the relationship between **Fasting Stabilized Glucose** and **Glycated Hemoglobin**,

---

## 🔑 Key Insights & Analytics

* **Stabilized Glucose vs. Glycated Hemoglobin:** There metrics have a positive 0.75 Pearson correlation, which shows their "symbiotic" relationship. Moreover, using Linear Regression and standard clinical thresholds (**126 mg/dL** for fasting glucose and **6.5%** for HbA1c), the analysis highlights strong concordance in extreme ranges, while isolating discordant cases (e.g., acute glucose spikes vs. chronic hyperglycemia).
* **Central Adiposity Impact:** Scatter plots and correlation metrics reveal a strong upward trend between waist circumference and HbA1c levels, illustrating the role of visceral fat in metabolic risk.
* **Age-Related Progression:** Demographic breakdown shows a marked shift in HbA1c density crossing the **6.5%** threshold past the age of 50, whereas younger cohorts (20–40) stay predominantly in the healthy range.

---

## 🛠️ Tech Stack & Workflow

* **Python:** Data ingestion (`kagglehub`), deduplication, string normalization, missing value imputation using age-group medians (`groupby` + `transform`), and feature creation (`age_group`).
* **Power BI & DAX:** Custom data modeling, interactive scatter plots with diagnostic quadrant reference lines, distribution histograms, and DAX measures for patient classification.
* **Data Sources:** [University of Virginia Rural Health Diabetes Dataset.](https://www.kaggle.com/datasets/imtkaggleteam/diabetes/data)

---

## 📊 Dashboard Visuals Overview

1. **Correlation Matrix & Variable Distributions:** Pearson correlation matrix mapping body measurements against metabolic markers alongside individual metric histograms.

<img width="1994" height="991" alt="1" src="https://github.com/user-attachments/assets/06297ff2-53c3-4650-a8c2-3b31642786e6" />

2. **Diagnostic Matrix (HbA1c vs. Fasting Glucose):** Scatter plot segmented into 4 clinical quadrants to evaluate diagnostic agreement and flag anomalies.

<img width="1458" height="1013" alt="2" src="https://github.com/user-attachments/assets/8e183944-d8fd-47f3-b35e-f4c17d3121c5" />

3. **Anthropometric & Demographic Risk Drivers:** Bivariate analyses evaluating HbA1c progression across waist measurements and age brackets.

<img width="1983" height="782" alt="3" src="https://github.com/user-attachments/assets/4f93c097-2f17-4629-8a9f-4f873568b731" />

---

## 🚀 How to Run

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/](https://github.com/)luipmesquita/Diabetes-Risk-Clinical-Biomarkers-Analysis.git
