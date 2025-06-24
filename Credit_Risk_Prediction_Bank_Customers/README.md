# 🏦 Credit Score Prediction – Bank GoodCredit

## 📘 Project Overview

This project aims to build a **machine learning model** that predicts the creditworthiness of credit card customers for **Bank GoodCredit**. The model classifies customers as **Good** or **Bad** based on historical data, enabling the bank to proactively manage credit risk and reduce default rates.

---

## 🎯 Business Objective

- Assess the **credit risk** of current credit card holders.
- Identify high-risk customers early to reduce **loan defaults**.
- Use predictive modeling to **automate credit scoring** and enhance decision-making.

---

## 🧾 Dataset Description

The data is sourced from a **MySQL relational database** and includes the following tables:

| Table Name           | Description                                          |
|----------------------|------------------------------------------------------|
| `Cust_Account`       | Credit card account history and repayment behavior   |
| `Cust_Enquiry`       | Credit inquiries made by customers                   |
| `Cust_Demographics`  | Personal and demographic information                 |

### 🏷️ Target Variable: `Bad_label`

- `0`: Good credit history  
- `1`: Bad credit history (customer falls into **30+ Days Past Due**)

---

## 🧠 Domain Context

Credit scoring is a fundamental task in the **financial and banking industry**. A customer's credit score indicates their **likelihood of default**, which directly impacts loan decisions. The solution developed here mimics the **internal credit risk assessment** process using data-driven methods.

---

## 🧰 Tech Stack & Tools

| Category          | Tools & Libraries                      |
|------------------|----------------------------------------|
| Language         | Python 3.x                              |
| Database         | MySQL                                   |
| Data Analysis    | Pandas, NumPy                           |
| Visualization    | Matplotlib, Seaborn                     |
| ML Libraries     | Scikit-learn, XGBoost, Imbalanced-learn |
| Database Access  | `mysql-connector-python`                |

---

## 🔄 Project Workflow

### 1. 🗄️ Data Extraction
- Connected to MySQL server using `mysql-connector-python`
- Queried and loaded data into Pandas DataFrames

### 2. 🔍 Exploratory Data Analysis (EDA)
- Analyzed data distributions, patterns, and outliers
- Visualized key relationships and correlations
- Treated missing values and encoded categorical features

### 3. 🏗️ Feature Engineering
- Merged data from multiple tables
- Created derived variables to capture customer behavior
- Normalized and scaled numerical features

### 4. 🤖 Model Development
- Built classification models to predict `Bad_label`
- Addressed class imbalance using **SMOTE** or **Resampling**
- Evaluated performance using:
  - **Accuracy**
  - **Precision & Recall**
  - **ROC-AUC**
  - **Confusion Matrix**

### 5. 📊 Insights & Recommendations
- Identified behavioral factors associated with bad credit
- Suggested monitoring features for real-time risk tracking
- Delivered a deployable predictive solution for credit scoring

---


---

## ✅ Outcomes

- Built an **end-to-end machine learning pipeline**
- Integrated **SQL + Python** for real-world data processing
- Developed an interpretable, high-performing credit risk model
- Applicable in live banking environments for **risk management**

---

## 📬 Contact

For queries or collaborations, connect via [LinkedIn](https://www.linkedin.com/in/bhaviksharma/)

---

