# 🩺 End-to-End Diabetes Risk Analytics & Clinical Strategy

A comprehensive healthcare analytics project leveraging **Python (Pandas, Seaborn, Matplotlib)** and **clinical feature engineering** across 47,541 patient records, paired with an executive presentation deck translating statistical findings into healthcare policy decisions.

---

## 📌 Executive Summary
* **Cohort Size:** 47,541 initial records audited; 13,257 quarantined due to physiological anomalies (e.g., diastolic BP ≥ systolic BP, extreme BMI artifacts); final clean cohort: **34,284 patients**.
* **Core Takeaway:** While genetic history incurs an average risk penalty of **+9.7 points**, optimized lifestyle factors (physical activity and diet quality) recover up to **12.0 points**, demonstrating that modifiable behaviors outweigh inherited predispositions.

---

## 🔬 Key Clinical Questions & Discoveries

1. **Diagnostic Biomarkers vs. Physical Markers:**
   * Fasting Blood Sugar (>140 mg/dL) and HbA1c categorized 87.3% of high-risk patients.
   * BMI exhibited negligible direct linear correlation with HbA1c ($r = -0.006$), confirming that weight alone is an inadequate proxy for glycemic risk without biochemical screening.
2. **Behavioral Thresholds:**
   * Physical activity levels and diet quality showed a steep "cliff" rather than a linear gradient: moving a patient out of the "Low/Poor" category yielded the entire measurable risk reduction (~11-12 percentage points).
3. **Age Progression:**
   * Risk increases across young adulthood and middle age (18–59) but plateaus after age 60 (mean score: ~78.9), indicating intervention programs must target individuals before age 60.

---

## 📊 Analytics Workflow
* **Data Wrangling:** Imputation of missing lipid values, mathematical derivation of height/weight from BMI ratios.
* **Feature Engineering:** 
  * `Unhealthy_Habits_Score` (0 to 7) combining physical inactivity, sleep deficits, and nutritional flags.
  * `Condition_Count` (0 to 5) aggregating hypertension, cardiovascular disease, and metabolic comorbidities.
* **Exploratory Data Analysis (EDA):** Multi-factor cross-tabulations, distributions, kernel density estimations (KDE), and correlation matrices.

---

## 🛠️ Tech Stack & Deliverables
* **Analysis & Modeling:** Python, Pandas, NumPy, Seaborn, Matplotlib.
* **Artifacts:**
  * Interactive Notebook: [Diabetes_Risk_Analysis.ipynb](Diabetes_Risk_Analysis.ipynb)
* Executive Slide Deck: [Diabetes_Risk_Analysis_Deck.pptx](Diabetes_Risk_Analysis_Deck.pptx)
* * Executive Slide Deck: [Diabetes_Risk_Analysis_Deck.pdf](Diabetes_Risk_Analysis_Deck.pdf)
