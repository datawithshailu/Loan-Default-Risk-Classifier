# 🏦 Loan Default Risk Classifier

**📈 Predicting loan defaults using Python, Exploratory Data Analysis (EDA), and Machine Learning**

---

## 🚀 Project Overview

Financial institutions face significant losses when customers default on loans. This project builds an **end-to-end data analysis and machine learning pipeline** to help predict which applicants are most likely to default on their loans.

Using a real-world dataset of loan applications, we:

✅ Explored and cleaned the data  
✅ Identified default patterns using EDA  
✅ Built machine learning models (Logistic Regression, Random Forest)  
✅ Handled data imbalance using smart techniques  
✅ Evaluated model accuracy and business impact

This project simulates how a **real data analyst in the finance industry** would approach a risk reduction problem.

---

## 🎯 Problem Statement

> Can we predict whether a loan applicant is likely to default (1) or not (0), based on their credit profile, income, loan type, and other details?

---

## 🛠 Tools & Technologies Used

| Category | Tools |
|---------|-------|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn (Logistic Regression, Random Forest) |
| Data Preparation | One-hot Encoding, Train-Test Split |
| Evaluation | Accuracy, Confusion Matrix, Precision/Recall, F1 Score |

---

## 📁 Dataset Details

- Rows: 148,000+
- Target column: `Status` → 0 = No Default, 1 = Default

### 🔑 Features include:
- `loan_amount`, `income`, `credit_score`, `property_value`
- `loan_purpose`, `term`, `rate_of_interest`, `age`, `employment type`, etc.

---

## 🧠 Step-by-Step Process

### 📌 Step 1: Data Loading & Initial Inspection
- Loaded the CSV file using Pandas
- Inspected column types, data ranges, missing values

### 🧹 Step 2: Data Cleaning
- Filled missing values (categorical → 'Unknown', numeric → median)
- Converted string columns to numerical using One-Hot Encoding
- Removed data inconsistencies and verified null counts

### 📊 Step 3: Exploratory Data Analysis (EDA)
- Analyzed which features affect loan defaults
- Visualized distributions of `income`, `loan_amount`, `credit_score`, and more
- Compared defaulters vs. non-defaulters across different categories

Key observations:
- Defaulters had lower income and credit scores
- Certain loan purposes (e.g. refinancing) had higher default risk
- Longer loan terms didn’t always mean higher risk

### ⚙️ Step 4: Feature Engineering
- Applied One-Hot Encoding to categorical columns
- Selected relevant numerical and categorical features
- Split data into train/test sets using `train_test_split()`

### 🤖 Step 5: Model Building
- Model 1: **Logistic Regression**  
    Basic model, showed weak recall due to data imbalance
- Model 2: **Random Forest Classifier** with `class_weight='balanced'`  
    Handled class imbalance better and captured more defaulters

### 📈 Step 6: Evaluation
- Evaluated with:
  - Confusion Matrix
  - Accuracy Score
  - Classification Report (Precision, Recall, F1-score)

---

## ✅ Final Results

| Metric              | Score |
|---------------------|--------|
| **Accuracy**        | 73.5% |
| **Recall (Defaulters)** | 17% |
| **Precision (Defaulters)** | 40% |
| **True Defaulters Detected** | 1,892 |

👉 These results show the model can **assist banks in identifying risky applicants** ahead of time — enabling safer loan decisions and reducing potential losses.

---

## 📌 Business Impact

- Helped improve loan approval accuracy
- Detected hidden defaulters that standard scoring may miss
- Reduces financial risk by using data to assist underwriters

---

## 📊 Sample Visuals

*(Include screenshots of bar plots, heatmaps, and model evaluation if uploading to GitHub)*

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `Loan_Default_Risk_Classifier_Polished.ipynb` | Complete Jupyter notebook with code and outputs |
| `README.md` | This documentation |

---

## 🙋‍♂️ Author

**Shailu**  
Aspiring Data Analyst | Focused on building real-world business-ready data projects.  
📬 [LinkedIn profile (add yours here)](https://www.linkedin.com)

---

## ⭐ Highlights for Recruiters

✅ Real-world domain: **Finance / Risk Analytics**  
✅ Clear data cleaning, EDA, modeling steps  
✅ Good use of visuals and logic  
✅ Focused on **explainability, results, and business impact**  
✅ Ready for interview discussion or portfolio demo

---

> ✨ Built as part of a learning journey to become a confident, job-ready data analyst.

