# 📈 Predictive Churn Analytics: Driving Retention at Tolson Tech

**Project Focus:** Developing a high-accuracy Machine Learning solution to identify and mitigate critical customer churn risks in an E-Commerce environment.

***

## 🌟 Executive Summary: Problem Solved

| Business Problem | Technical Solution | Business Result |
| :--- | :--- | :--- |
| **17%** E-Commerce Customer Churn Rate | **Decision Tree Classifier** optimized for recall | **90.3%** accuracy in predicting high-value, at-risk customers. |

***

## 🛠️ Core Technical Skills

| Area | Technologies & Techniques |
| :--- | :--- |
| **Languages** | Python (Pandas, NumPy) |
| **Data Analysis** | Exploratory Data Analysis (EDA), Feature Engineering, Correlation Analysis |
| **Modeling** | **Decision Tree Classifier (Selected)**, Logistic Regression, Hyperparameter Tuning |
| **ML Metrics** | **Recall ($\uparrow$ Critical)**, Accuracy, Precision, F1 Score, Confusion Matrix |
| **Data Prep** | Median Imputation, Label/One-Hot Encoding, StandardScaler |

***

## 💡 Top 3 Actionable Findings (The "Why")

The analysis isolated key customer segments driving the highest churn, enabling targeted retention strategies:

| Churn Driver | Churn Rate | Recommendation Focus |
| :--- | :--- | :--- |
| **1. Early-Stage Volatility** | **29.0%** (Tenure $\le 5$ months) | Immediate Proactive Onboarding Campaigns |
| **2. Regional/Product Risk** | **42.2%** (Tier 3 customers buying Mobile Phones) | Deep-dive on regional supply chain and product quality assurance. |
| **3. Logistics Friction** | **21.0%** (Warehouse Distance $\text{26-50}$ units) | Introduce priority shipping or localized fulfillment options. |

***

## 🏆 Model Performance & Selection

The goal was to maximize **Recall** to ensure minimal missed churners (False Negatives). The Decision Tree model was selected for production use.

| Model | Accuracy | Precision | **Recall** | F1 Score |
| :--- | :--- | :--- | :--- | :--- |
| Baseline: Logistic Regression | 90.4% | 80.8% | 54.6% | 65.2% |
| **Final: Decision Tree** | **96.98%** | **91.26%** | **90.27%** | **90.76%** |

***

## 💻 Project Execution

The complete analysis, data cleaning workflow, EDA visualizations, and model training/comparison are documented in the following Jupyter Notebook:

### How to Run

1.  **Clone the repository.**
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  **Open the notebook:**
    ```bash
    jupyter notebook Group-6.ipynb
    ```
