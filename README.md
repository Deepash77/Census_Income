# Census Income Prediction

## 📌 Project Overview

This project uses Machine Learning to predict whether an individual earns more than $50K per year based on demographic, educational, occupational, and financial attributes.

The project follows an end-to-end Data Science workflow:

Data Cleaning → EDA → Feature Engineering → Model Building → Model Evaluation → Hyperparameter Tuning → Business Insights

---

## 🎯 Problem Statement

The objective is to build a classification model that predicts an individual's income category.

- `0` → Income <= $50K
- `1` → Income > $50K

The project uses the Census Income dataset containing information about more than 48,000 individuals.

---

## 💡 Solution

The project implements multiple Machine Learning algorithms:

1. Logistic Regression
2. Decision Tree
3. Random Forest

The models are compared using Accuracy, Precision, Recall, F1 Score, and ROC-AUC.

---

## 📊 Dataset

The dataset contains features such as:

- Age
- Workclass
- Education
- Occupation
- Marital Status
- Relationship
- Race
- Sex
- Capital Gain
- Capital Loss
- Hours per Week
- Native Country
- Income

Dataset Source:

UCI Machine Learning Repository  
https://archive.ics.uci.edu/ml/datasets/census+income

---

## 🔍 Exploratory Data Analysis

The following analysis was performed:

- Missing value analysis
- Duplicate record analysis
- Outlier detection
- Income distribution
- Age distribution
- Education vs Income
- Occupation vs Income
- Workclass vs Income
- Capital Gain analysis
- Correlation analysis

---

## 🧹 Data Preprocessing

The following preprocessing techniques were used:

- Handling missing values
- Removing duplicate records
- Outlier analysis
- Encoding categorical variables
- Feature scaling
- Train-test split

---

## 🤖 Machine Learning Models

### Logistic Regression

Used as the baseline classification model.

### Decision Tree

Used to capture non-linear relationships between features.

### Random Forest

Used as an ensemble learning model to improve prediction performance.

---

## 📈 Model Performance

| Model | ROC-AUC |
|---|---:|
| Logistic Regression | 0.9025 |
| Decision Tree | 0.8950 |
| Random Forest | 0.9044 |
| Final Tuned Model | 0.9118 |

---

## 🏆 Final Model Results

| Metric | Score |
|---|---:|
| Accuracy | 85.51% |
| Precision | 80.15% |
| Recall | 55.60% |
| F1 Score | 65.65% |
| ROC-AUC | 91.18% |

The final model achieved a ROC-AUC of **91.18%**, showing strong ability to distinguish between the two income classes.

---

## 🔎 Classification Report

| Class | Precision | Recall | F1 Score |
|---|---:|---:|---:|
| Income <= $50K | 0.87 | 0.95 | 0.91 |
| Income > $50K | 0.80 | 0.56 | 0.66 |

The model performs strongly for the <=$50K class, while the recall for the >$50K class indicates room for further improvement.

---

## 💼 Target Industries

This project demonstrates techniques relevant to:

- FinTech
- Banking
- Digital Lending
- Insurance
- E-Commerce
- Customer Analytics
- Risk Analytics
- Workforce Analytics

### Potential FinTech Applications

The methodology can be adapted for:

- Customer segmentation
- Income estimation
- Financial profiling
- Risk analytics
- Product recommendation
- Credit pre-screening

> Note: Real financial applications would require additional financial data, fairness testing, regulatory compliance, and privacy controls.

---

## 🧠 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📁 Project Structure

```text
census-income-prediction/
│
├── data/
│   └── census-income.csv
│
├── notebooks/
│   └── Census_Income_Analysis.ipynb
│
├── images/
│   ├── income_distribution.png
│   ├── correlation_heatmap.png
│   ├── model_comparison.png
│   └── confusion_matrix.png
│
├── requirements.txt
└── README.md
