# 📊 Customer Churn Prediction & EDA

### 📘 Project Overview

This project focuses on understanding customer behavior and predicting **churn likelihood** in a banking environment.
By performing detailed **Exploratory Data Analysis (EDA)** and **machine learning classification**, the goal is to help businesses reduce customer loss and improve retention strategies.

### 🎯 Objective

To perform **EDA** to uncover churn-driving patterns and build a **classification model** that predicts which customers are likely to leave the bank.

### 🧩 Dataset

**Source:** Publicly available banking dataset
**Size:** 10,000 records, 14 columns
**Target Variable:** `Exited` → (1 = Customer left, 0 = Customer retained)

**Key Features:**

* Demographic: `Gender`, `Geography`, `Age`, `Tenure`
* Financial: `CreditScore`, `Balance`, `NumOfProducts`, `HasCrCard`, `EstimatedSalary`
* Behavioral: `IsActiveMember`, `Exited`

### ⚙️ Data Preprocessing

* Dropped unnecessary columns (`RowNumber`, `CustomerID`, `Surname`)
* Handled outliers using **IQR method**
* **Label Encoding** for binary features, **One-Hot Encoding** for categorical features
* 80:20 Train-Test Split with **Stratified Sampling**

### 🔍 Exploratory Data Analysis (EDA)

**Univariate Insights**

* Most customers are aged **30–40 years**
* ~**20%** churn rate (imbalanced dataset)
* Majority credit scores between **600–700**

**Bivariate & Multivariate Insights**

* **Older and inactive** customers show higher churn
* **German customers** churn more than French or Spanish
* High-balance customers have a **greater churn risk**
* Correlation heatmap shows **Age (+0.29)** and **IsActiveMember (–0.16)** as key drivers

### 🤖 Machine Learning Model

**Algorithms Tested:** Logistic Regression, Decision Tree, Random Forest, XGBoost
**Final Model:** Tuned Logistic Regression
**ROC-AUC:** ≈ 0.77

### 💡 Key Results

* Identified **high-risk churn segments**
* Revealed that **inactive and high-balance customers** are likely to leave
* Model achieved strong balance between accuracy and interpretability

### 🏢 Business Impact

* Enabled **targeted retention campaigns**
* Helped identify high-value customers at risk
* Guided **region-specific strategies** and improved customer engagement

### 🛠️ Tools & Libraries

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn

### 📈 Future Enhancements

* Apply **SMOTE** or **class weights** for imbalance handling
* Deploy as a **Flask web app** for interactive predictions
* Integrate with Power BI for churn monitoring dashboards

---
