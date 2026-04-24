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

## 📊 Visualizations & Output Graphs

> **📌 How to Add Your Graphs:**
> 1. Run the Jupyter notebook to generate the plots
> 2. Right-click on each plot and select "Save Image As"
> 3. Save them as `waterfront_boxplot.png` and `sqft_above_regplot.png`
> 4. Create an `images/` folder in your repository
> 5. Upload both images to the `images/` folder
> 6. The graphs will automatically appear below

---

### 🌊 Figure 1: Waterfront vs. Non-Waterfront House Prices

**Code:**
```python
plt.figure(figsize=(10, 6))
sns.boxplot(x='waterfront', y='price', data=df)
plt.title('House Prices: Waterfront vs Non-Waterfront')
plt.xlabel('Waterfront View (0=No, 1=Yes)')
plt.ylabel('Price')
plt.show()
<img width="833" height="547" alt="1" src="https://github.com/user-attachments/assets/c350cd5e-b074-4eb3-99b6-a71232a42e21" />

---
📐 Figure 2: Correlation Between Above-Ground Square Footage and Price
Code:
plt.figure(figsize=(10, 6))
sns.regplot(x='sqft_above', y='price', data=df)
plt.title('Correlation between Sqft_Above and Price')
plt.xlabel('Square Feet Above Ground')
plt.ylabel('Price')
plt.show()
<img width="833" height="547" alt="2" src="https://github.com/user-attachments/assets/7a65f444-a8c6-4096-bba1-b16e214eff8d" />
