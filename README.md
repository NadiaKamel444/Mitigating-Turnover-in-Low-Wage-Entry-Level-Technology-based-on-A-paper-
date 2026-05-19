# Mitigating-Turnover-in-Low-Wage-Entry-Level-Technology-based-on-A-paper-
Business Problem Technology organizations that rely on low-wage, entry-level positions often suffer from high employee turnover rates, with many employees leaving within their first six months of employment. This constant churn leads to several negative consequences
# 📊 Mitigating Turnover in Low-Wage Entry-Level Technology Roles

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)
[![Data Analytics](https://img.shields.io/badge/Fields-HR%20Analytics%20%7C%20Data%20Science-orange)](https://github.com/)
[![Statistical Test](https://img.shields.io/badge/Test-Independent%20T--Test-green)](https://github.com/)

An HR Analytics project focused on evaluating the impact of **Skill-Based Incentive Programs** on employee retention and mitigating high turnover rates within low-wage, entry-level technology positions.

---

## 📌 Project Overview
Technology organizations relying on low-wage, entry-level roles often experience severe employee attrition, with a high percentage of new hires leaving within their first six months. This study analyzes a dataset of **200 employees over an 18-month period** to measure how structured skill development plans influence employee tenure and stabilize the workforce.

### 📉 The Problem & Business Impact
Constant employee churn leads to:
1. **Increased Recruitment Costs:** High expenses related to continuously sourcing talent.
2. **High Training Expenses:** Sunk costs in onboarding and basic training for short-tenured hires.
3. **Decreased Productivity:** Extended vacancies or roles filled by inexperienced staff.
4. **Team Burnout:** Increased workload on remaining team members, triggering further turnover.

---

## 🛠️ Methodology & Dataset

### Dataset Variables
The analysis monitors the following metrics for 200 employees:
* `Age` / `Gender` / `Education` / `Job Role` / `Salary`
* `Tenure (Months)`: Calculated based on Hire and Exit dates.
* `Program Participation`: Binary indicator (`1` = Participant, `0` = Non-Participant).
* `Training Completion %`
* `Performance Score`

### Data Preparation Steps
1. **Turnover Target Mapping:** Created a binary target variable where `1` indicates the employee left during the study, and `0` indicates active employment.
2. **Population Segmentation:** Segmented the workforce into two core experimental groups: **Program Participants** vs. **Non-Participants**.

---

## 🔬 Statistical Analysis & Results

An **Independent T-Test** was conducted to compare the mean tenure between program participants and non-participants.

### 📈 Key Findings
* **T-Statistic:** `16.83`
* **P-Value:** `< 0.001`
* **Statistical Conclusion:** The extremely low p-value allows the confident rejection of the null hypothesis ($H_0$), proving a statistically significant relationship between the incentive program and tenure extension.

### 💡 Key Insights
1. **Doubled Tenure:** Program participants remained with the company for **more than double** the duration of non-participants.
2. **Dramatically Reduced Turnover:** Program engagement is linked to a **>30% reduction** in the turnover rate.
3. **Clear ROI Potential:** Structured skill incentives directly correlate with improved job stability and employee loyalty, offering a concrete path to minimizing attrition costs.

---

## 🚀 Business Recommendations
1. **Transition to Core Strategy:** Shifting the program from optional to a core, strongly encouraged component of the entry-level employee value proposition.
2. **Link Training to Tangible Rewards:** Formalizing promotions, salary step-ups, and internal mobility options based on training completion and performance scores.
3. **Integrate Long-Term Retention:** Embedding the framework into the broader organizational culture to foster continuous learning.

---

## 📂 Repository Structure
```text
├── data/
│   └── employees_dataset.csv     # Simulated/Anonymized HR Data (200 records)
├── notebooks/
│   └── hr_turnover_analysis.ipynb # Statistical test execution and visualizations
├── src/
│   └── main_analysis.py          # Pure Python script for end-to-end analysis
├── README.md                     # Project documentation
└── requirements.txt              # Software dependencies
