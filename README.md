# 🛒 Customer Lifetime Value (CLTV) Prediction System

A Machine Learning project that predicts the Customer Lifetime Value of eCommerce customers using RFM (Recency, Frequency, Monetary) features and Regression models.

## 🌐 Live Demo
👉 **[Click here to try the Live CLTV Predictor](https://kishansingh7x.github.io/Customer-Lifetime-Value-Prediction)**

> Enter any customer's Recency, Frequency and Monetary values and instantly get their predicted Customer Lifetime Value!

---

## 📌 Project Overview

Every business wants to know — **which customers are most valuable?**  
This project answers that by predicting how much revenue a customer will generate over their lifetime, using real eCommerce behavioral data.

---

## 📊 Dataset

- **Source:** [eCommerce Behavior Data from Multi Category Store — Kaggle](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store)
- **File Used:** `2019-Oct.csv.gz` (October 2019)
- **Size:** 40+ lakh events
- **Unique Customers:** 3,43,646
- **Key Columns:** `event_type`, `user_id`, `price`, `event_time`, `user_session`

---

## 🧠 Methodology

### 1. Data Preprocessing
- Filtered only `purchase` events (revenue-generating)
- Removed missing values and invalid prices
- Converted timestamps to datetime format

### 2. Feature Engineering — RFM Model
| Feature | Description |
|---|---|
| **Recency** | Days since last purchase |
| **Frequency** | Number of unique sessions |
| **Monetary** | Total amount spent |

### 3. Machine Learning Models Trained
| Model | R² Score |
|---|---|
| Random Forest ⭐ Best | 1.0000 |
| Gradient Boosting | 0.9980 |
| Ridge Regression | 0.9210 |
| Linear Regression | 0.9190 |
| Lasso Regression | 0.9150 |

### 4. Evaluation Metrics
- **R² Score** — measures how well model explains variance
- **MAE** — Mean Absolute Error
- **RMSE** — Root Mean Squared Error

---

## 🏆 Results

- **Best Model:** Random Forest Regressor
- **R² Score:** 1.0000
- **MAE:** 0.0000
- **RMSE:** 0.0001

---

## 📁 Project Structure
customer-lifetime-value-prediction/
├── CLTV_Prediction.ipynb     # Main Jupyter Notebook
├── demo.html                 # Live interactive demo
├── eda_plots.png             # EDA visualizations
├── correlation_heatmap.png   # Feature correlation
├── model_comparison.png      # Model comparison chart
├── actual_vs_predicted.png   # Best model results
├── feature_importance.png    # Feature importance chart
└── README.md                 # Project documentation

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/customer-lifetime-value-prediction.git
cd customer-lifetime-value-prediction
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 3. Download the dataset
Download `2019-Oct.csv.gz` from [Kaggle](https://www.kaggle.com/datasets/mkechinov/ecommerce-behavior-data-from-multi-category-store) and place it in the project folder.

### 4. Run the notebook
```bash
jupyter notebook CLTV_Prediction.ipynb
```

### 5. Open the live demo
Simply double-click `demo.html` — opens in any browser, no server needed.

---

## 🖥️ Live Demo Features

- Enter Recency, Frequency, Monetary values manually
- Or click preset buttons (VIP / Regular / Inactive / New Customer)
- Instantly see predicted CLTV and customer segment
- View feature contribution breakdown
- See all 5 model R² scores

---

## 🛠️ Technologies Used

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data-green)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red)

- **Python 3.10**
- **Pandas** — Data manipulation
- **NumPy** — Numerical computing
- **Matplotlib & Seaborn** — Data visualization
- **Scikit-learn** — Machine learning models
- **Jupyter Notebook** — Development environment
- **HTML/CSS/JavaScript** — Live demo interface

---

## 👤 Author

**Kishan** — AI/ML Exhibition Project 2026  
📧 kishansingh7x@gmail.com  
🔗 [GitHub](https://github.com/kishansingh7x)

---
