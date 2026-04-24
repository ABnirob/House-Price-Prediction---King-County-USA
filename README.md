# 🏠 House Price Prediction - King County, USA

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-1.3.4-green.svg)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-0.20.1-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

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
| Polynomial (deg=2) + Ridge | 0.80 |

---

## 🗂️ Dataset

**Source:** King County house sales (Kaggle, modified for coursework)

**Size:** 21,613 records × 21 features

### Features

| Feature | Description |
|---------|-------------|
| `price` | Target variable - house sale price |
| `sqft_living` | Square footage of the home |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `floors` | Total floors in house |
| `waterfront` | Waterfront view (0/1) |
| `grade` | Overall grade (King County system) |
| `lat` / `long` | Geographic coordinates |
| `sqft_above` | Square footage above basement |

---

## 🚀 Getting Started

### Run on Google Colab

[![Open In Colab](https://colab.research.google.com/drive/10YawmlL0SEGwrfJk6GPH8VGqc4kPRejl#scrollTo=TrHqHMCqhMYS)

### Local Installation

```bash
# Clone repository
git clone https://github.com/ABnirob/House-Price-Prediction---King-County-USA.git
cd house-price-prediction

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Launch notebook
jupyter notebook House_Sales_Prediction.ipynb
