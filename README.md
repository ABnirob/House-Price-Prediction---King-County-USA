# 🏡 House Sales in King County, USA | Predictive Analysis & Visualization

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-FA0F00?logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.5-F7931E?logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.2-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.13-388E3C?logo=python&logoColor=white)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.10-11557C?logo=python&logoColor=white)](https://matplotlib.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📊 Project Overview

This project performs an **exploratory data analysis (EDA)** and **predictive modeling** on housing data from **King County, USA** (Seattle metropolitan area). The goal is to uncover key factors influencing house prices and build regression models to predict property values accurately.

As a **Data Analyst**, I transformed raw real estate data into actionable insights, identifying which features most strongly correlate with price and quantifying their impact using **Linear Regression**.

---

## 🎯 Project Objectives

| # | Objective | Status |
|---|-----------|--------|
| 1 | Clean and preprocess the dataset (handle missing values, remove unnecessary columns) | ✅ Complete |
| 2 | Explore price distribution across key categorical features (e.g., waterfront view) | ✅ Complete |
| 3 | Visualize correlations between continuous features (sqft_above, price) | ✅ Complete |
| 4 | Build a **Simple Linear Regression** model to predict price using `sqft_living` | ✅ Complete |
| 5 | Build a **Multiple Linear Regression** model using multiple features | ✅ Complete |
| 6 | Evaluate model performance using **R² Score** | ✅ Complete |

---

## 🧰 Tools & Technologies Used

| Category | Tools |
|----------|-------|
| **Data Manipulation** | Pandas, NumPy |
| **Data Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-learn (LinearRegression) |
| **Environment** | Jupyter Notebook / Google Colab |

---

## 📁 Dataset Description

**Source:** King County House Sales Dataset (IBM Data Science Course)

**Key Features:**

| Column | Description |
|--------|-------------|
| `price` | Target variable (house price in USD) |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `sqft_living` | Square footage of living space |
| `floors` | Number of floors |
| `waterfront` | Waterfront view (1 = yes, 0 = no) |
| `view` | Quality of view (0-4 scale) |
| `grade` | Construction grade (1-13 scale) |
| `sqft_above` | Square footage above ground |
| `lat` | Latitude coordinate |

---

## 🔍 Exploratory Data Analysis (EDA)

### Data Cleaning Performed:
- ✅ Removed unnecessary columns (`id`, `Unnamed: 0`)
- ✅ Handled missing values in `bedrooms` and `bathrooms` using mean imputation

### Data Cleaning Code:
```python
# Remove unnecessary columns
df.drop(['id', 'Unnamed: 0'], axis=1, inplace=True)

# Handle missing values with mean imputation
mean_bedrooms = df['bedrooms'].mean()
mean_bathrooms = df['bathrooms'].mean()
df['bedrooms'].fillna(mean_bedrooms, inplace=True)
df['bathrooms'].fillna(mean_bathrooms, inplace=True)

# Verify no missing values remain
print("Missing values in bedrooms:", df['bedrooms'].isnull().sum())
print("Missing values in bathrooms:", df['bathrooms'].isnull().sum())
