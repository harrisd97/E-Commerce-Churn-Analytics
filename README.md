# 📈 Churn Analytics: E-Commerce Customer Retention Analysis

---

## 💡 Project Goal

The objective of this project was to identify and analyze the primary factors driving customer churn for an e-commerce platform. Using **Exploratory Data Analysis (EDA)** and **Machine Learning**, we developed a predictive model to accurately flag at-risk customers and provided actionable strategies to improve customer retention.

---

## 🧹 Data Cleaning & Pre-processing

The initial dataset (5,630 records) contained missing values and inconsistent categorical labels.

### Key Cleaning Steps

1.  **Missing Data Imputation:** Missing values (ranging from 4.46% to 5.45% of the data) in all numerical columns (`Tenure`, `WarehouseToHome`, etc.) were filled using the **median** due to skewed distributions.
2.  **Categorical Standardization:** Inconsistent values were unified (e.g., 'Phone' $\rightarrow$ 'Mobile Phone'; 'COD' $\rightarrow$ 'Cash on Delivery').
3.  **Feature Engineering:** Four high-impact flag features were created based on EDA patterns, including:
    * `ShortTenureFlag` ($\leq 5$ months)
    * `Tier3_MobilePhone` (Highest churn interaction)

---

## 📊 Exploratory Data Analysis (EDA) - Key Insights

The overall churn rate for the platform is **17%**. Analysis focused on identifying specific segments with the highest risk:

| High-Risk Segment | Churn Rate | Primary Driver/Insight |
| :--- | :--- | :--- |
| **New Customers** | **29.0%** (Tenure 0-5 months) | High early-stage volatility and low initial loyalty. |
| **"Satisfied" Churners** | **24.0%** (Satisfaction Score 5) | External/unaccounted operational issues, despite high survey satisfaction. |
| **Logistics Risk** | **21.0%** (Distance 26-50 units) | Likely impacted by delivery times or cost due to warehouse distance. |
| **Single, Low-Commitment Payments** | **42.7% - 44.4%** | Single customers using Cash on Delivery or E-Wallet show extreme churn risk. |
| **Tier 3 Mobile Shoppers** | **42.2%** | Highest single interaction risk, suggesting regional supply/delivery challenges. |

---

## 🤖 Model Performance & Selection

We compared Logistic Regression (LR) with a Decision Tree (DT) model, prioritizing **Recall** to ensure maximum identification of true churners.

### Evaluation Summary

| Metric | Logistic Regression (LR) | Decision Tree (DT) |
| :--- | :--- | :--- |
| **Accuracy** | 90.4% | **96.98%** |
| **Precision** | 80.8% | **91.26%** |
| **Recall (CRITICAL)** | 54.6% | **90.27%** |
| **F1 Score** | 65.2% | **90.76%** |

The **Decision Tree model** is the preferred solution, offering a dramatic improvement in **Recall** (from 54.6% to **90.3%**), making it highly effective for targeted retention efforts.

---

## ✅ Actionable Retention Strategies

Based on the highest-impact churn factors, the following recommendations are key to reducing the 17% churn rate:

* **Proactive Onboarding:** Launch a personalized engagement and support program immediately for **new customers ($\leq 5$ months tenure)** to mitigate early-stage volatility.
* **Logistics Optimization:** Enhance delivery speed or offer discounted shipping for customers in the **26-50 unit distance** range.
* **Deep Customer Feedback:** Investigate the reasons behind churn among **highly satisfied customers (Score 5)**, potentially through qualitative feedback, to uncover hidden pain points.
* **Payment Incentives:** Promote committed payment methods (Credit/Debit Card) to the **Single_COD_EWallet** group with exclusive loyalty benefits or small-value cashback offers.
