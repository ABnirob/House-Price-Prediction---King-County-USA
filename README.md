# 🏠 House Price Prediction — King County, USA

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-FA0F00?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.5-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.2-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.13-388E3C?logo=python&logoColor=white)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.10-11557C?logo=python&logoColor=white)](https://matplotlib.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
---

## 📌 Executive Summary

This project delivers an end-to-end predictive analysis of residential property prices in **King County, USA** using regression modeling techniques.

The objective was to:
- Identify key drivers of housing prices  
- Quantify relationships between property features and price  
- Build a robust predictive model with strong generalization performance  

> ✅ Final Model Performance: **R² = 0.80**  
> 📈 Achieved using **Polynomial Features + Ridge Regularization**

---

## 🎯 Business Problem

Accurate house price estimation is critical for:
- Real estate valuation
- Investment decision-making
- Market trend analysis

This project addresses the challenge of modeling **non-linear relationships** in housing data while avoiding overfitting.

---

## 📊 Dataset

- **Source:** King County housing dataset  
- **Time Range:** May 2014 – May 2015  
- **Scope:** Residential property sales (including Seattle)

### Key Features:
- `sqft_living` — Living area size  
- `bedrooms`, `bathrooms`  
- `floors`  
- `waterfront`  
- `condition`, `grade`  
- `sqft_above`, `sqft_basement`  

---

## 🧠 Analytical Approach

### 1. Data Preparation
- Removed irrelevant identifiers (`id`, `Unnamed: 0`)
- Handled missing values via mean imputation
- Validated data consistency

### 2. Exploratory Data Analysis
- Distribution analysis of price and key variables  
- Outlier detection (waterfront vs price)  
- Correlation analysis to identify predictive features  

### 3. Modeling Strategy

| Model | Purpose |
|------|--------|
| Simple Linear Regression | Baseline performance |
| Multiple Linear Regression | Multivariate relationships |
| Pipeline (Scaling + LR) | Standardized workflow |
| Ridge Regression | Regularization |
| Polynomial + Ridge | Non-linear modeling |

---

## 📈 Model Performance
Model Comparison (R² Score)
Simple Linear (sqft_living) 0.49
Multiple Linear Regression 0.70
Pipeline (Scaled LR) 0.68
Ridge Regression 0.68
Polynomial + Ridge 0.80

---


### ✅ Final Model:
**Polynomial Features (degree = 2) + Ridge Regression**

**Why it works:**
- Captures non-linear feature interactions  
- Reduces variance via regularization  
- Improves generalization on unseen data  

---

## 🔍 Key Insights

- 📈 Property size (`sqft_living`) is the strongest predictor of price  
- 🌊 Waterfront properties significantly increase valuation  
- 🧩 Feature interactions (non-linear effects) materially improve predictions  
- ⚖️ Regularization is essential to prevent overfitting in complex models  

---

## 📸 Visual Outputs

| Analysis | Visualization |
|---------|--------------|
| Waterfront vs Price |(<img width="833" height="547" alt="1" src="https://github.com/user-attachments/assets/249e2cb7-142a-4694-b673-84f2fd48991b" />
) |
| sqft_above vs Price | (<img width="833" height="547" alt="2" src="https://github.com/user-attachments/assets/8fc219d3-ef0f-4888-9ca7-e8f86d555b83" />
) |

---

## 🛠️ Tech Stack

- **Languages:** Python  
- **Libraries:**  
  - Pandas, NumPy  
  - Matplotlib, Seaborn  
  - Scikit-Learn  

- **ML Techniques:**  
  - Regression Modeling  
  - Feature Engineering  
  - Regularization (Ridge)  
  - Polynomial Transformation  
  - Pipeline Optimization  

 ```bash
👨‍💻 Author
Md Abul Bashar Nirob
📌 Aspiring Data Analyst | Machine Learning Enthusiast
GitHub: https://github.com/ABnirob
LinkedIn: https://www.linkedin.com/in/md-abul-bashar-nirob/
```

 
 


