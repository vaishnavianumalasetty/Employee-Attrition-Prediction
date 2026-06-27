# 🧠 Employee Attrition Prediction & Prevention System

![Python](https://img.shields.io/badge/Python-3.14-blue)
![PowerBI](https://img.shields.io/badge/PowerBI-Dashboard-yellow)
![ML](https://img.shields.io/badge/ML-Logistic%20Regression-green)
![SQL](https://img.shields.io/badge/SQL-SQLite-orange)

## 📌 Project Overview
An end-to-end Employee Attrition Prediction system built using Python, SQL, and Power BI. This project predicts which employees are likely to leave the organization, identifies key attrition drivers, calculates business impact, and provides actionable retention recommendations.

---

## 🎯 Problem Statement
Employee attrition costs companies 6 months of an employee's salary per departure. This project analyzes IBM HR Analytics data of 1,470 employees across 35 variables to:
- Predict at-risk employees before they leave
- Identify top factors driving attrition
- Quantify financial impact
- Recommend targeted retention strategies

---

## 🛠️ Tools & Technologies
| Category | Tools |
|---|---|
| Language | Python 3.14 |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Database | SQLite |
| BI Dashboard | Microsoft Power BI |
| IDE | VS Code + Jupyter Notebook |

---

## 📁 Project Structure

## 📁 Project Structure
```
Employee-Attrition-Prediction/
├── data/
│   └── processed/
│       └── attrition_cleaned.csv
├── notebooks/
│   ├── 01_EDA.ipynb
│   └── 02_ML_Model.ipynb
├── outputs/
│   ├── 01_attrition_distribution.png
│   ├── 02_attrition_by_department.png
│   ├── 03_attrition_by_overtime.png
│   ├── 04_attrition_by_age.png
│   ├── 05_attrition_by_income.png
│   ├── 06_attrition_by_jobsatisfaction.png
│   ├── 07_correlation_heatmap.png
│   ├── 08_attrition_by_tenure.png
│   ├── 09_attrition_by_worklifebalance.png
│   ├── 10_attrition_by_distance.png
│   ├── 11_lr_confusion_matrix.png
│   ├── 12_model_comparison.png
│   ├── 13_feature_importance.png
│   ├── retention_recommendations.csv
│   ├── page1_attrition_overview.png
│   ├── page2_predictive_insights.png
│   └── page3_retention_recommendations.png
└── README.md
```

---

## 📊 Dataset
- **Source:** IBM HR Analytics Employee Attrition Dataset
- **Size:** 1,470 employees × 35 variables
- **Target:** Attrition (Yes/No)
- **Features:** Age, Department, MonthlyIncome, OverTime, JobSatisfaction, YearsAtCompany, and 29 more

---

## 🔍 Key Findings from EDA

| # | Finding |
|---|---|
| 1 | Overall attrition rate: **16.12%** (237/1470 employees) |
| 2 | Overtime employees are **3x more likely** to leave |
| 3 | Employees aged **25-35** have highest attrition |
| 4 | Employees who left earned **₹2,505 less** per month |
| 5 | Low satisfaction employees have **22.7% attrition rate** |
| 6 | Employees in first **1-2 years** are most at risk |
| 7 | Long commute employees leave significantly more |

---

## 🤖 ML Model Results

| Model | Accuracy | Recall | F1 Score | ROC-AUC |
|---|---|---|---|---|
| Logistic Regression (Basic) | 86.73% | 36.17% | 46.58% | 66.26% |
| Random Forest (Balanced) | 83.67% | 29.79% | 36.84% | 61.86% |
| Random Forest (Tuned) | 82.65% | 36.17% | 40.00% | 63.83% |
| **LR Tuned (Best)** | **75.17%** | **76.60%** | **49.66%** | **75.75%** |

### ✅ Best Model: Logistic Regression (Tuned)
- Recall of **76.60%** — catches 3 out of 4 at-risk employees
- ROC-AUC of **75.75%** — strong overall model quality

---

## 🏆 Top 10 Attrition Drivers
1. MonthlyIncome ← #1 factor!
2. Age
3. TotalWorkingYears
4. DailyRate
5. HourlyRate
6. MonthlyRate
7. DistanceFromHome
8. YearsAtCompany
9. OverTime
10. NumCompaniesWorked

---

## 💰 Business Impact

| Metric | Value |
|---|---|
| Total Employees Analyzed | 294 |
| 🔴 High Risk Employees | 75 |
| 🟡 Medium Risk Employees | 78 |
| 🟢 Low Risk Employees | 141 |
| Total Potential Loss | ₹59,69,690 |
| **Savings if 30% Retained** | **₹17,90,907** |

---

## 📋 Retention Recommendations

| Risk Level | Action |
|---|---|
| 🔴 High Risk + Overtime | Immediate intervention — reduce overtime + salary review |
| 🔴 High Risk | Urgent — schedule retention meeting + growth plan |
| 🟡 Medium Risk | Monitor closely — offer development opportunities |
| 🟢 Low Risk | Maintain current engagement |

---

## 📈 Power BI Dashboard
3-page interactive dashboard:
- **Page 1:** Attrition Overview — KPIs, dept analysis, age groups
- **Page 2:** Predictive Insights — Risk distribution, top drivers
- **Page 3:** Retention Recommendations — Action plan + savings

### Dashboard Preview
#### Page 1 — Attrition Overview
![Page1](outputs/page1_attrition_overview.png)

#### Page 2 — Predictive Insights
![Page2](outputs/page2_predictive_insights.png)

#### Page 3 — Retention Recommendations
![Page3](outputs/page3_retention_recommendations.png)

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/vaishnavianumalasetty/Employee-Attrition-Prediction

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn jupyter ipykernel

# 3. Run notebooks in order
# Open notebooks/01_EDA.ipynb first
# Then open notebooks/02_ML_Model.ipynb

# 4. Open dashboard
# Open Employee_Attrition_Dashboard.pbix in Power BI Desktop
```

---

## 👩‍💻 Author
**Vaishnavi Anumalasetty**
- 🔗 [LinkedIn](https://linkedin.com/in/vaishnavi-anumalasetty-171b51320)
- 🐙 [GitHub](https://github.com/vaishnavianumalasetty)
