# 🏠 House Price Prediction - King County, USA

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3.4-green.svg)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-0.20.1-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red.svg)](https://jupyter.org/)

> A comprehensive data analytics project predicting residential property prices using regression models on the King County housing dataset.

---

## 📊 Project Overview

This project analyzes **house sale prices in King County, USA** (including Seattle) from **May 2014 to May 2015**. As a **Data Analyst** at a Real Estate Investment Trust (REIT), I developed predictive models to determine market prices based on property features such as square footage, bedrooms, floors, waterfront views, and more.

### Key Results

| Model | R² Score |
|-------|----------|
| Simple Linear (sqft_living) | 0.49 |
| Multiple Linear Regression | 0.70 |
| Pipeline (Scaler + LR) | 0.68 |
| Ridge Regression (α=0.1) | 0.68 |
| Polynomial (deg=2) + Ridge | **0.80** |

---

## 📸 Output Pictures

### 1. Data Types & Summary Statistics
![Data Types](output_images/dtypes.png)
*Displaying data types of each column using `df.dtypes`*

### 2. Statistical Summary After Dropping Columns
![Describe](output_images/describe.png)
*Statistical summary after dropping 'id' and 'Unnamed: 0' columns*

### 3. Floor Value Counts
![Floors Value Counts](output_images/floors_counts.png)
*Unique floor values transformed into DataFrame using `value_counts().to_frame()`*

### 4. Boxplot: Waterfront vs Price Outliers
![Boxplot](output_images/boxplot.png)
*Comparison of price outliers for houses with and without waterfront views*
- ✅ Houses with waterfront view have **higher median prices**
- ✅ Houses without waterfront view have **more outliers**

### 5. Regplot: sqft_above vs Price Correlation
![Regplot](output_images/regplot.png)
*Positive correlation between above-ground square footage and sale price*

### 6. Linear Regression Results (sqft_living)
![Linear Regression](output_images/linear_regression.png)
*R² = 0.4935 for sqft_living predicting price*

### 7. Multiple Linear Regression Results
![Multiple Linear Regression](output_images/multiple_linear.png)
*R² = 0.7009 using 11 features*

### 8. Pipeline Results
![Pipeline](output_images/pipeline.png)
*Pipeline with StandardScaler + Linear Regression: R² = 0.6847*

### 9. Ridge Regression Results
![Ridge](output_images/ridge.png)
*Ridge (alpha=0.1): R² = 0.6841*

### 10. Polynomial + Ridge Results
![Polynomial Ridge](output_images/polynomial_ridge.png)
*Polynomial (degree=2) + Ridge: R² = 0.8012*

### 11. Final Summary of All R² Scores
![Summary](output_images/summary.png)
*Comparison of all model performances*

---

## 🗂️ Dataset

**Source:** King County house sales (Kaggle, modified for coursework)

**Size:** 21,613 records × 21 features

### Features Description

| Feature | Description |
|---------|-------------|
| `price` | Target variable - house sale price |
| `sqft_living` | Square footage of the home |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `floors` | Total floors in house |
| `waterfront` | Waterfront view (0=No, 1=Yes) |
| `view` | View quality rating |
| `condition` | House condition rating |
| `grade` | Overall grade (1-13) |
| `sqft_above` | Square footage above basement |
| `sqft_basement` | Basement square footage |
| `yr_built` | Year built |
| `yr_renovated` | Year renovated |
| `zipcode` | ZIP code |
| `lat` / `long` | Geographic coordinates |
| `sqft_living15` | Living room area in 2015 |
| `sqft_lot15` | Lot size area in 2015 |

---

## 🚀 Getting Started

### Run on Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

### Local Installation

```bash
# Clone repository
git clone https://github.com/yourusername/house-price-prediction.git
cd house-price-prediction

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Launch Jupyter Notebook
jupyter notebook House_Sales_Prediction.ipynb
