# Predictive Churn Analytics

**Project Focus:** Developing and comparing Machine Learning models to predict customer churn for an E-Commerce business, with a focus on maximizing the identification of at-risk customers.

---

## Project Summary

This project addresses the critical business problem of customer churn. By analyzing customer data, we built and evaluated two models to predict which customers are likely to leave. The final model, a **Decision Tree Classifier**, achieved high accuracy and recall, enabling the business to proactively target at-risk customers with retention campaigns.

| Business Problem | Technical Solution | Key Result |
| :--- | :--- | :--- |
| **17%** Customer Churn Rate | **Decision Tree Classifier** optimized for recall. | **97%** accuracy in predicting churn, with **90%** of actual churners correctly identified. |

---

## Technical Skillset

This project demonstrates proficiency in the end-to-end machine learning workflow, from data cleaning and feature engineering to model training and evaluation.

| Area | Technologies & Techniques |
| :--- | :--- |
| **Languages** | Python (Pandas, NumPy, Scikit-learn) |
| **Data Analysis** | Exploratory Data Analysis (EDA), Feature Engineering, Correlation Analysis |
| **Modeling** | **Decision Tree Classifier (Selected)**, Logistic Regression |
| **ML Metrics** | **Recall (Optimized)**, Accuracy, Precision, F1 Score, Confusion Matrix |
| **Data Preprocessing** | Median Imputation, Label & One-Hot Encoding, StandardScaler |

---

## Top 3 Actionable Insights

The analysis isolated three key drivers of customer churn, providing clear focus areas for retention strategies.

| Churn Driver | Churn Rate | Recommendation |
| :--- | :--- | :--- |
| **1. Early-Stage Customers** | **29.0%** (Tenure ≤ 5 months) | Implement proactive onboarding and engagement campaigns for new customers. |
| **2. Regional & Product Issues** | **42.2%** (Tier 3 city customers buying Mobile Phones) | Investigate regional logistics and product satisfaction for this specific segment. |
| **3. High-Risk Segments** | **44.4%** (Single customers using E-wallet) | Offer targeted promotions or alternative payment benefits for this demographic. |

---

## Model Performance & Selection

The primary goal was to maximize **Recall**, ensuring that the fewest possible at-risk customers were missed. While both models performed well, the **Decision Tree Classifier** was selected for its superior balance of precision and high recall.

| Model | Accuracy | Precision | **Recall** | F1 Score |
| :--- | :--- | :--- | :--- | :--- |
| Baseline: Logistic Regression | 90.4% | 80.8% | 54.6% | 65.2% |
| **Final: Decision Tree** | **97.0%** | **91.3%** | **90.3%** | **90.8%** |

---

## Project Walkthrough

The complete analysis, including data cleaning, exploratory visualizations, and model training, is documented in the accompanying Jupyter Notebook.

### How to Run Locally

1.  **Clone the repository.**
2.  **Install the required dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  **Launch Jupyter Notebook and open the file:**
    ```bash
    jupyter notebook "Group-6.ipynb"
    ```
