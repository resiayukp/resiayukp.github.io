---
title: Projects
permalink: /projects/
---

[Home](/) · [Projects](/projects/) · [Experience](/experience/) · [Contact](/#contact)

# Projects

## Volve Field Production Analytics Dashboard

**Tools:** Power BI, DAX, Power Query · **Code:** [GitHub repository](https://github.com/resiayukp/volve-field-production-analytics-dashboard)

**Problem.** Production data is spread across many wells and periods, which makes it hard to see which wells drive output, where production is declining and how injection relates to production.

**What I built.** A four-page Power BI dashboard on Equinor's open Volve dataset:

1. Executive Summary: field KPIs for oil, gas, water and water injection, producer and injector counts, top performer well.
2. Production and Injection Performance: trends over time, top producing wells, water cut.
3. Well Spatial Analysis: surface and bottom-hole coordinates with production by well.
4. Business Insights: top performing, declining and high water cut wells.

**How.** Star-schema data model, DAX measures for KPIs and time intelligence, and data cleaning and validation in Power Query.

!\[Executive Summary page](/assets/img/volve-executive-summary.PNG)

\---

## Symptom-Based Illness Classification

**Tools:** Python, pandas, scikit-learn, XGBoost · **Code:** [GitHub repository](https://github.com/resiayukp/symptom-classification-logistic-regression)

**Problem.** Predict COVID, flu, cold or allergy from 20 yes/no symptoms when COVID and cold are only about 7% of the data. The dataset is synthetic, so this is a modeling exercise, not a clinical tool.

**What I did.** Compared eight classification algorithms (KNN, Logistic Regression, SVC, Decision Tree, Random Forest, Gradient Boosting, XGBoost and a neural network) on 44,453 records, tuning each with cross-validated grid search.

**Findings.**

* Class weighting raised COVID recall from 0.52 to 0.95 and COLD recall from 0.64 to 1.00, while accuracy stayed at 0.93. Balanced accuracy rose from 0.77 to 0.96.
* Six models made identical predictions at the dataset's accuracy ceiling of about 93%, so I chose Logistic Regression as the simplest, fastest and most interpretable option.
* Test results: accuracy 0.932, balanced accuracy 0.956, macro F1 0.812. Precision for COLD and COVID is about 0.5, which means many false alarms for those two classes.

\---

