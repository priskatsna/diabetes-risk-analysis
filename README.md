# Early Stage Diabetes Risk Analysis using UCI Dataset

## Project Summary

This project presents an in-depth **Exploratory Data Analysis (EDA)** on the Early Stage Diabetes Risk Prediction dataset, aimed at identifying symptoms and patterns associated with diabetes diagnosis. The project was developed for a **university-level Big Data Management midterm exam** and includes a combination of univariate and multivariate visualizations to uncover meaningful insights.

## 📁 Dataset

[![UCI Dataset](https://img.shields.io/badge/UCI%20Dataset-Diabetes%20Risk-orange?logo=data)](https://archive.ics.uci.edu/dataset/529/early+stage+diabetes+risk+prediction+dataset)

### ⭐ Situation

Diabetes is a serious public health issue worldwide. Early detection plays a vital role in improving treatment outcomes and life expectancy. In this context, real patient data from the Sylhet Diabetes Hospital in Bangladesh has been collected to assist in identifying early-stage diabetes risks through symptom-based analysis.

### ⭐ Task

The main objectives of this project were:
- To perform a comprehensive univariate and multivariate analysis of patient data.
- To understand the distribution and correlation of key symptoms related to diabetes.
- To interpret which attributes contribute strongly to a positive diabetes diagnosis.
- To use visual exploration to support early detection strategies.

### ⭐ Action

- Dataset sourced from UCI with **520 samples** and **17 features** (16 predictors + 1 target).
- Features include both demographic (e.g., Age, Gender) and clinical symptoms (e.g., Polyuria, Polydipsia, Obesity).
- Performed univariate analysis using:
  - Histograms and density plots for numeric feature (`Age`)
  - Bar plots and frequency tables for categorical and binary features
  - Boxplots for visualizing spread and outliers
- Conducted multivariate analysis using:
  - Correlation heatmap (after encoding binary features to 0/1)
  - Scatter plots and joint plots (Age vs. Class)
  - Swarm plots, violin plots, and box plots (Age vs. symptom categories)
  - Count plots (symptoms vs. diagnosis class)
- Visualizations used libraries such as `matplotlib`, `seaborn`, and `pandas`.

### ⭐ Result

- Most patients are aged **30–60**, with a peak at 50–60 years.
- Binary features like **Polyuria**, **Polydipsia**, and **Sudden Weight Loss** show **positive correlation** with diabetes.
- Variables like **Gender** and **Alopecia** show weak or no correlation with the diagnosis.
- Class distribution:
  - 320 patients are labeled `Positive` (risk of diabetes)
  - 200 patients are labeled `Negative`
- Dataset quality is high, with very few missing values (1.3% in `Thal`, 0.6% in `Ca`).
- Limitation: only **1 numeric variable (Age)** restricts complex multivariate numeric analyses.

## 📊 Key Insights

- Patients aged 40–55 dominate the data range and are the highest risk group.
- `Polyuria`, `Polydipsia`, and `Sudden Weight Loss` are **strong indicators** of positive diagnosis.
- Features such as `Visual Blurring` and `Delayed Healing` also contribute but to a lesser extent.
- Features like `Obesity` and `Alopecia` show **low predictive importance**.
