# Diabetes-Risk-Clinical-Biomarkers-Analysis

## 📌 Executive Summary

When assessing diabetes risk, there's one clinical metric that stands out in evaliation, and that is 𝐆𝐥𝐲𝐜𝐚𝐭𝐞𝐝 𝐇𝐞𝐦𝐨𝐠𝐥𝐨𝐛𝐢𝐧 (also known as HbA1c). But what about (Fasting) 𝐒𝐭𝐚𝐛𝐢𝐥𝐢𝐳𝐞𝐝 𝐆𝐥𝐮𝐜𝐨𝐬𝐞 and anthropometric attributes?

In my latest end-to-end data project, I analyzed clinical data from the University of Virginia Rural Health Dataset using 𝐏𝐲𝐭𝐡𝐨𝐧 and 𝐏𝐨𝐰𝐞𝐫 𝐁𝐈 to evaluate diabetes diagnostic concordance between 𝐆𝐥𝐲𝐜𝐚𝐭𝐞𝐝 𝐇𝐞𝐦𝐨𝐠𝐥𝐨𝐛𝐢𝐧 and 𝐒𝐭𝐚𝐛𝐢𝐥𝐢𝐳𝐞𝐝 𝐆𝐥𝐮𝐜𝐨𝐬𝐞, and physical risk drivers.

---

## 🔑 Key Insights & Analytics

1 - 𝐒𝐭𝐚𝐛𝐢𝐥𝐢𝐳𝐞𝐝 𝐆𝐥𝐮𝐜𝐨𝐬𝐞 vs. 𝐆𝐥𝐲𝐜𝐚𝐭𝐞𝐝 𝐇𝐞𝐦𝐨𝐠𝐥𝐨𝐛𝐢𝐧: These metrics have a positive 0.75 Pearson correlation, which shows their "symbiotic" relationship. Using standard clinical thresholds (126 mg/dL for fasting glucose and 6.5% for HbA1c), the 4-quadrant scatter analysis reveals strong diagnostic alignment in extreme ranges. However, it also isolates critical outliers—such as acute glucose spikes vs. chronic hyperglycemia.

2 - 𝐈𝐦𝐩𝐨𝐫𝐭𝐚𝐧𝐜𝐞 𝐨𝐟 𝐚𝐧𝐭𝐡𝐫𝐨𝐩𝐨𝐦𝐞𝐭𝐫𝐢𝐜 𝐚𝐭𝐭𝐫𝐢𝐛𝐮𝐭𝐞𝐬: 
2.1 - There is a clear upward trend between Waist Circumference and elevated HbA1c, illustrating the direct role of visceral fat in insulin resistance.
2.2 - Age-Related Progression breakdown shows a marked increase in HbA1c density crossing the 6.5% threshold past the age of 50, while younger cohorts (ages 20–40) remain predominantly in the healthy range.

---

## 🛠️ Tech Stack & Workflow

𝐏𝐲𝐭𝐡𝐨𝐧 : Data ingestion (kagglehub), cleaning, normalization, and age-group median imputation.
𝐏𝐨𝐰𝐞𝐫 𝐁𝐈 & 𝐃𝐀𝐗: Custom data modeling, interactive diagnostic quadrant scatter plots, and distribution analysis.

---

## 🔑 Key Insights & Analytics

* **Stabilized Glucose vs. Glycated Hemoglobin:** These metrics have a positive 0.75 Pearson correlation, which shows their "symbiotic" relationship. Moreover, using Linear Regression and standard clinical thresholds (**126 mg/dL** for fasting glucose and **6.5%** for HbA1c), the analysis highlights strong concordance in extreme ranges, while isolating discordant cases (e.g., acute glucose spikes vs. chronic hyperglycemia).
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
