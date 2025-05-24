# 💼 Bankruptcy Prediction Using Financial Ratios (SAS EM)

This project, completed as part of **MGMT 571: Data Mining** at Purdue University, focuses on building predictive models to forecast corporate bankruptcy based on financial ratio data. Using a dataset of over 18,000 companies and 64 financial attributes, we explored various machine learning techniques in **SAS Enterprise Miner** to develop robust classifiers for early bankruptcy warning.

---

## 🧠 Problem Statement

The goal was to accurately predict whether a firm would go bankrupt (binary classification: `0 = Not Bankrupt`, `1 = Bankrupt`) using historical financial ratios such as:

- Net Profit / Total Assets  
- Total Liabilities / Total Assets  
- Gross Margin, Return on Equity, etc.

Out of 18,000 firms:
- **9,789** did not go bankrupt  
- **211** did go bankrupt  
> ⚠️ Highly imbalanced dataset

---

## 📊 Dataset Overview

| Feature | Description |
|---------|-------------|
| Size | 18,000 observations |
| Features | 64 financial ratios |
| Target Variable | `Class` (0 = healthy, 1 = bankrupt) |
| Missing Values | None |

---

## ⚙️ Modeling Approach

### 🔄 Preprocessing
- Variable selection  
- Sampling strategies  
- Normalization and transformations  
- Feature filtering using LASSO and stepwise regression

### 🏗️ Models Built
- Logistic Regression (Forward, Backward, Stepwise)  
- Decision Trees  
- Neural Networks  
- Gradient Boosting  
- HP Tree (High Performance)  
- Ensemble Models

### 🧪 Evaluation Metrics
- **ROC Curve (Validation)**: 0.909  
- **ROC Curve (Test - Public)**: 0.94472  
- **ROC Curve (Test - Private)**: 0.94013  

---

## 🧬 Final Models

| Model | Composition | Public ROC | Private ROC |
|-------|-------------|------------|-------------|
| **Model I** | Gradient Boosting + Backward Regression + Neural Network | 0.94303 | 0.94145 |
| **Model II** | Gradient Boosting + Backward Regression + Neural Network + HP Tree | **0.94472** | 0.94013 |

---

## 🧠 Key Learnings

- **Preprocessing isn’t always beneficial**—especially in clean datasets  
- **Ensembling** can significantly boost performance when individual models are strong  
- **Precision-Recall** analysis is crucial for imbalanced datasets  
- **Validation ROC** is helpful, but not always the full picture  

---

## 👥 Team

- Darshan Upadhyay  
- Ananth Mohan  

(DARing ANAlysts)

---

## 📄 Files Included

- `Data Mining Final Project.pdf` – Business-style summary presentation of the project  
- (Optional) Add your `.sas7bdat` or model export files here if public

---

## 📌 Tools Used

- **SAS Enterprise Miner**  
- Excel / Python (for sanity checks)  
- Tableau (if visualizations were used)

---

> 💬 For questions, contact **upadhy33@purdue.edu**
