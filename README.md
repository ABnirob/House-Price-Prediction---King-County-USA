# 🏠 House Price Prediction — King County, USA

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3+-green.svg)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange.svg)](https://scikit-learn.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success.svg)]()

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
| Waterfront vs Price | ![](output_images/boxplot.png) |
| sqft_above vs Price | ![](output_images/regplot.png) |
| Model Summary | ![](output_images/summary.png) |

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

```bash
📝 Conclusion
Summary of Findings
This analysis successfully demonstrates that:

✅ Waterfront location is a powerful predictor of higher house prices, with waterfront properties showing significantly higher median values and wider price distribution.

✅ Square footage (both living and above-ground) shows a positive correlation with price, though the relationship is not perfectly linear.

✅ Multiple linear regression (R² = 0.660) significantly outperforms simple linear regression (R² = 0.493), demonstrating a 33.9% improvement in predictive accuracy.

✅ Feature selection matters — location (latitude), construction grade, number of bathrooms, and view quality are important price drivers beyond just square footage.

Business Value
The models built serve as a solid foundation for:

🏢 Automated Home Valuation Systems - Quick, data-driven price estimates

📊 Investment Decision Support - Identify undervalued properties

🎯 Targeted Marketing - Focus on high-value buyer segments

📈 Market Trend Analysis - Track price drivers over time

Limitations & Future Work
Limitation	Future Enhancement
66% of price variance explained	Add zip code, school ratings, crime data
Linear models only	Test non-linear algorithms (Random Forest, XGBoost)
No temporal analysis	Include time-series features (sale date, market trends)
Missing property condition data	Add renovation history, condition scores
```
 


