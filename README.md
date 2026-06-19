# 🏠 House Price Prediction using Machine Learning

<div align="center">

**Regression-Based Real Estate Price Prediction & Data Analysis**

**Author:** **Shrishti Vaishnav**

![Python](https://img.shields.io/badge/Python-3.x-blue?style=for-the-badge\&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green?style=for-the-badge\&logo=pandas)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge\&logo=scikitlearn)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-blueviolet?style=for-the-badge)

</div>

---

# 📌 Project Overview

The real estate market depends heavily on accurate property valuation for buyers, sellers, investors, and developers. Manual estimation methods often rely on subjective judgment and outdated comparisons, leading to inconsistent pricing decisions.

This project develops a **Machine Learning-based House Price Prediction System** that estimates property prices using structural and location-based features such as:

* 📐 Area
* 🛏️ Bedrooms
* 🛁 Bathrooms
* 🏢 Stories
* 🚗 Parking
* ❄️ Air Conditioning
* 📍 Preferred Area
* 🛋️ Furnishing Status

The project follows a complete Data Science workflow, including **data exploration, preprocessing, regression modeling, visualization, model evaluation, and business insight generation**.

---

# 🎯 Objectives

* Load and explore a real-world housing dataset.
* Clean and preprocess data for machine learning.
* Encode categorical variables using One-Hot Encoding.
* Build and compare multiple regression models.
* Evaluate prediction performance using standard regression metrics.
* Visualize relationships between property features and prices.
* Generate actionable business insights for the real estate industry.

---

# 📂 Dataset

**Dataset:** Housing Prices Dataset

The dataset contains information about residential properties and their selling prices.

### Dataset Statistics

| Attribute         | Value     |
| ----------------- | --------- |
| Total Records     | **545**   |
| Original Features | **13**    |
| Target Variable   | **price** |
| Missing Values    | **0**     |
| Duplicate Records | **0**     |

---

# 🛠️ Technology Stack

| Technology       | Purpose                     |
| ---------------- | --------------------------- |
| Python           | Programming Language        |
| Jupyter Notebook | Development Environment     |
| Pandas           | Data Loading & Manipulation |
| NumPy            | Numerical Operations        |
| Scikit-Learn     | Machine Learning Models     |
| Matplotlib       | Data Visualization          |
| Seaborn          | Statistical Visualization   |

---

# 📋 Project Workflow

```
Housing Dataset
        │
        ▼
Data Loading & Exploration
        │
        ▼
Data Cleaning & Preprocessing
        │
        ▼
Feature Encoding
        │
        ▼
Train-Test Split (80:20)
        │
        ▼
Model Building
 ├── Linear Regression
 └── Random Forest Regressor
        │
        ▼
Model Evaluation
(MAE • RMSE • R² Score)
        │
        ▼
Data Visualization
        │
        ▼
Business Insights & Recommendations
```

---

# 📊 Data Preprocessing

The preprocessing pipeline included:

* ✅ Missing value verification
* ✅ Duplicate record detection
* ✅ One-Hot Encoding of categorical variables
* ✅ Feature preparation for regression models

### Categorical Variables Encoded

* mainroad
* guestroom
* basement
* hotwaterheating
* airconditioning
* prefarea
* furnishingstatus

Final processed dataset:

**545 Rows × 14 Features**

---

# 🤖 Machine Learning Models

Two supervised regression algorithms were implemented and benchmarked.

## 1️⃣ Linear Regression

A statistical regression algorithm that models the relationship between independent variables and house prices using a linear equation.

### Performance

| Metric                  | Value             |
| ----------------------- | ----------------- |
| Mean Absolute Error     | **$970,043.40**   |
| Root Mean Squared Error | **$1,324,506.96** |
| R² Score                | **0.6529**        |

---

## 2️⃣ Random Forest Regressor

An ensemble learning algorithm that combines multiple decision trees to improve prediction stability and reduce variance.

### Performance

| Metric                  | Value             |
| ----------------------- | ----------------- |
| Mean Absolute Error     | **$1,021,546.04** |
| Root Mean Squared Error | **$1,400,565.97** |
| R² Score                | **0.6119**        |

---

# 📈 Model Comparison

| Metric   | Linear Regression | Random Forest |
| -------- | ----------------- | ------------- |
| MAE      | $970,043.40       | $1,021,546.04 |
| RMSE     | $1,324,506.96     | $1,400,565.97 |
| R² Score | **0.6529**        | **0.6119**    |

### 🏆 Best Performing Model

**Linear Regression**

It achieved:

* Lower prediction error
* Better generalization
* Higher R² Score

making it the preferred model for this dataset.

---

# 📉 Visualizations

The project includes three analytical visualizations:

### 📊 Distribution of House Prices

* Histogram with Kernel Density Estimation
* Displays price distribution and median value

---

### 🔥 Correlation Heatmap

Illustrates relationships among all encoded features and identifies the strongest predictors of house prices.

---

### 🎯 Actual vs Predicted Scatter Plot

Compares Random Forest predictions against actual prices using an ideal reference line to evaluate prediction quality.

---

# 🔍 Key Insights

### 🏡 Area is the Strongest Predictor

Larger houses consistently command higher market prices.

---

### 🛁 Bathrooms Increase Property Value

Properties with additional bathrooms generally achieve significantly higher valuations.

---

### ❄️ Air Conditioning Adds Premium Value

Homes equipped with air conditioning exhibit noticeably higher selling prices compared to similar properties without it.

---

### 📍 Preferred Locations Matter

Properties located in preferred residential areas benefit from increased market demand and higher prices.

---

### 🏠 Guest Rooms & Basements Have Limited Impact

Contrary to common assumptions, these features demonstrate relatively weak individual influence on property valuation.

---

# 💼 Business Recommendations

For real estate developers, investors, and asset management firms:

### ✅ Prioritize

* Expanding living area
* Adding bathrooms
* Installing modern air conditioning
* Improving functional living space

### ❌ Lower Priority Investments

* Guest room additions
* Basement renovations

These improvements generate comparatively lower returns on investment.

---

# 📁 Project Structure

```
HousePricePrediction/

│── analysis.ipynb
│── Housing.csv
│── summary.pdf
│── README.md
│
└── charts/
    ├── chart1_price_distribution.png
    ├── chart2_correlation_heatmap.png
    └── chart3_actual_vs_predicted.png
```

---

# 🚀 How to Run

### Clone the repository

```bash
git clone https://github.com/yourusername/HousePricePrediction.git
```

### Navigate to the project directory

```bash
cd HousePricePrediction
```

### Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Launch Jupyter Notebook

```bash
jupyter notebook analysis.ipynb
```

---

# 📌 Conclusion

This project demonstrates an end-to-end machine learning workflow for predicting house prices using regression techniques. Through comprehensive data exploration, preprocessing, visualization, and model benchmarking, the analysis identified the most influential housing characteristics affecting property valuation.

Among the evaluated models, **Linear Regression achieved the highest predictive performance with an R² score of 0.6529**, explaining approximately **65% of the variance in house prices**. The findings illustrate how machine learning can support data-driven decision-making for real estate pricing, investment analysis, and property development strategies.

---

# 👩‍💻 Author

**Shrishti Vaishnav**

*Building intelligent solutions through data, machine learning, and analytics.*
