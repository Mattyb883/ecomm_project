# E-commerce Data Analysis & Dashboard Project

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![Looker Studio](https://img.shields.io/badge/Looker-Studio-4285F4?logo=google)
![XGBoost](https://img.shields.io/badge/XGBoost-Model-success)
![License](https://img.shields.io/badge/License-MIT-green)

This project analyzes an e-commerce dataset to uncover insights about sales, profit, product performance, and brand trends. It includes data preprocessing, exploratory data analysis (EDA), predictive modeling, and a fully interactive dashboard built in Looker Studio.

---

## Table of Contents

- [Dashboard Preview](#-dashboard-preview)
- [Dataset Overview](#dataset-overview)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Predictive Modeling](#predictive-modeling)
- [Looker Studio Dashboard](#looker-studio-dashboard)
- [Key Insights](#key-insights)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Author & License](#author--license)

---

## Dashboard Preview

![Dashboard KPI](images/dashboard_preview.png)

---

## Dataset Overview

- **Source**: [Kaggle – E-commerce Dataset](https://www.kaggle.com/datasets/risheejosi05/e-commerce-dataset)
- **Records**: 91,349 products
- **Fields**: Product name, brand, price, rating, discount, quantity, revenue, profit, and more.

---

## Data Preprocessing

- Cleaned and normalized columns
- Converted strings to lowercase, removed extra whitespace
- Simulated estimated cost and profit based on product category margin assumptions
- Imputed missing values where applicable
- Created engineered fields: quantity, revenue, profit margin

---

## Exploratory Data Analysis

Performed extensive EDA to understand:
- Best-performing brands by revenue and profit
- Top product categories by sales volume
- Correlations between discount %, revenue, and profit
- Margin efficiency by product tag

Charts and heatmaps created using `matplotlib` and `seaborn`.

---

## Predictive Modeling

### Model 1: Predict Quantity Sold
- **Model Used**: XGBoost Regressor
- **Features**: Discount %, Rating, Brand, Product Tag
- **Performance**:  
  - **R² Score**: 0.85  
  - **RMSE**: 339  
- **Outcome**: Accurately predicts demand based on key product signals

---

## Looker Studio Dashboard

> https://lookerstudio.google.com/s/nvHTKlW62F8

Built an interactive dashboard with:
- KPI scorecards
- Brand-level and product-tag-level visualizations
- Filters for brand and category
- Profitability and volume analysis

---

## Key Insights

- High-margin categories include **makeup** and **personal care**
- Most revenue comes from **watches** and **EDT gift sets**
- Strong correlation between quantity sold and revenue
- Margin efficiency varies widely by category

---

## Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, XGBoost)
- Jupyter Notebook
- Google Looker Studio
- GitHub for version control

---

## Project Structure

ecomm_project/
│
├── data.csv # Raw dataset from Kaggle
├── ecomm_analysis.ipynb # Jupyter notebook for EDA & modeling
├── dashboard_layout_mockup.pdf # Visual layout of the Looker dashboard
├── ecomm_final_data.csv # Cleaned dataset for Looker
├── images/
│ ├── dashboard_kpi.png # Screenshot of KPI section
│ └── dashboard_products.png # Screenshot of product insights
├── README.md # Project documentation (this file)

---

## Author & License

**Author**: Matt Baglietto  
Feel free to fork and build on this project for educational or portfolio use.

**License**: [MIT](LICENSE)
