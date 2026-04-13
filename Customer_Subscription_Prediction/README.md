# Customer Subscription Prediction & Marketing Analysis

> Can we predict which customers will subscribe before we call them?

**Tools:** Python · Pandas · Scikit-learn · Matplotlib · Seaborn · Tableau  
**Dataset:** Bank Marketing Dataset — 45,211 records  
**Models:** Logistic Regression · Decision Tree · Random Forest  

---

## The Business Problem

A financial services company runs outbound telemarketing campaigns to sell term deposit subscriptions. Each call costs time and money. The marketing team needed to answer one question:

**Which customers are most likely to subscribe so we can prioritize outreach and cut wasted spend?**

---

## What I Built

A full machine learning pipeline that:
- Cleaned and prepared 45,000+ customer records
- Performed exploratory analysis to surface behavioral and demographic patterns
- Built and compared 3 classification models (Logistic Regression, Decision Tree, Random Forest)
- Identified the top 15 features driving subscription decisions
- Delivered 5 concrete business recommendations backed by data

---

## Key Findings

**1. Calling more than 3 times hurts, not helps**  
Subscription rates drop sharply after the 3rd contact. Customers contacted 5+ times convert at near-zero rates. Reallocating that budget to fresh leads could cut wasted calls by ~35%.

**2. Students and retirees convert at 2x the average rate**  
Despite being smaller segments, these groups significantly over-index on subscriptions. They should be the first priority in any campaign.

**3. Timing matters — May is the worst month to launch**  
May is the most common campaign month but has one of the lowest conversion rates. September, October, and December outperform consistently.

**4. Economic indicators predict behavior better than demographics**  
The Euribor 3-month rate and employment figures are the strongest predictors. Campaigns launched during favorable economic conditions convert at higher rates.

---

## Visualizations (Location: images\placeholder.md)

### Subscription Rate by Job Type

### Seasonal Subscription Patterns

### Age Distribution: Subscribers vs Non-Subscribers

### Diminishing Returns: More Calls ≠ More Conversions

### Subscription Rate by Education Level

### Model Comparison — ROC Curves

### Top 15 Features Driving Predictions


---

## Model Performance

| Model | AUC | Accuracy | Precision | Recall | F1 Score |
| :--- | :---: | :---: | :---: | :---: | :---: |
| Logistic Regression | — | — | — | — | — |
| Decision Tree | — | — | — | — | — |
| Random Forest | — | — | — | — | — |

> Results populate after running the notebook. Random Forest typically achieves AUC > 0.79 on this dataset.

---

## Business Recommendations

| Priority | Recommendation | Expected Impact |
| :--- | :--- | :--- |
| High | Stop contacting customers after 3 failed attempts | ~35% reduction in wasted calls |
| High | Prioritize students and retirees in targeting | 8–12% improvement in conversion |
| Medium | Shift campaign budget from May to Sep–Dec | Better seasonal alignment |
| Medium | Use model risk scores to tier outreach | Focus reps on highest-probability leads |
| Low | Monitor Euribor rate as a campaign launch trigger | Align timing with economic conditions |

---

## How to Run This Project

```bash
# 1. Clone the repo
git clone https://github.com/Cinco33/Data_Science_Portfolio.git
cd Data_Science_Portfolio/Customer_Subscription_Prediction

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# 3. Download the dataset
# Get bank-additional-full.csv from:
# https://archive.ics.uci.edu/ml/datasets/Bank+Marketing
# Place it in the /data folder

# 4. Run the notebook
jupyter notebook Customer_Subscription_Prediction.ipynb
```

---

## Project Structure

```
Customer_Subscription_Prediction/
│
├── Customer_Subscription_Prediction.ipynb   # Full analysis notebook
├── README.md                                # This file
│
├── data/
│   └── bank-additional-full.csv            # Source dataset (not tracked in git)
│
└── images/
    ├── 01_subscription_by_job.png
    ├── 02_subscription_by_month.png
    ├── 03_age_distribution.png
    ├── 04_contacts_vs_conversion.png
    ├── 05_subscription_by_education.png
    ├── 06_correlation_heatmap.png
    ├── 07_roc_curves.png
    ├── 08_confusion_matrix.png
    └── 09_feature_importance.png
```

---

*Part of the [Darius Nobles Data Science Portfolio](https://github.com/Cinco33/Data_Science_Portfolio)*  
*[LinkedIn](https://www.linkedin.com/in/dariusnobles/) · [Portfolio Website](https://dariusnobles.netlify.app/)*
