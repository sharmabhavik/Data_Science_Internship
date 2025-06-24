# 🏃‍♂️ Human Activity Classification: Walking vs Running

Classifying human motion as **Walking** or **Running** using time-series sensor data and machine learning.  
📌 Built as part of the **Data Science Internship at [Rubixe™](https://rubixe.com/)**.

---

## 📚 Overview

With the increasing use of smart wearables and fitness trackers, identifying human activity from motion sensors is more valuable than ever.  
This project builds a robust machine learning pipeline to distinguish between walking and running using accelerometer data.

---

## 🧠 Tech Stack

- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
- **ML Algorithms:** K-Nearest Neighbors (KNN), Support Vector Machine (SVM), Random Forest, Logistic Regression  
- **Environment:** Jupyter Notebook

---

## 📊 Dataset Description

- Accelerometer readings along **X**, **Y**, **Z** axes  
- Timestamped activity labels: `Walking`, `Running`  
- Optional features: step frequency, stride length (if available)

🎯 **Target Variable:** `Activity` (`Walking` or `Running`)

---

## 🔄 Workflow

### 🔹 1. Data Preprocessing
- Cleaned missing or noisy values  
- Applied **sliding windows** and **rolling statistics**  
- Normalized feature values

### 🔹 2. Feature Engineering
- Extracted time-domain statistics: `mean`, `std`, `max`, `min`  
- Calculated **magnitude vectors** and frequency-domain components  
- Derived motion dynamics (derivatives)

### 🔹 3. Exploratory Data Analysis
- Visualized motion signals over time  
- 3D scatter plots for X-Y-Z patterns  
- t-SNE for clustering and dimensionality reduction

### 🔹 4. Model Building
- Baseline models: Logistic Regression, KNN  
- Advanced: Tuned SVM and Random Forest  
- Cross-validation used to avoid overfitting

### 🔹 5. Evaluation
- **Metrics:** Accuracy, Precision, Recall, F1-Score  
- **Tools:** Confusion Matrix, Classification Report  
- Activity-wise performance breakdown

---

## 📈 Model Performance

| Model                  | Accuracy | F1 Score |
|------------------------|----------|----------|
| Logistic Regression    | 0.85     | 0.84     |
| K-Nearest Neighbors    | 0.88     | 0.87     |
| Support Vector Machine | 0.91     | 0.90     |
| 🌟 **Random Forest**     | **0.94** | **0.93** |

✅ **Best Model:** `Random Forest Classifier`

