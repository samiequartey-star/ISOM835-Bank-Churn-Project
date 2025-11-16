# ISOM835-Bank-Churn-Project
# 🏦 Bank Customer Churn Prediction  
### ISOM 835 – Predictive Analytics & Machine Learning  
**Suffolk University | Sawyer Business School**  
Instructor: Hasan Arslan  

---

## 📌 Project Overview  
This project analyzes and predicts **bank customer churn** using machine learning techniques. Customer churn is an important business problem because retaining customers is far less costly than acquiring new ones.

The goal of this project is to:

- Explore customer behavioral and financial patterns  
- Build machine learning models to predict churn  
- Identify the key factors that influence churn  
- Provide actionable business recommendations  
- Discuss ethical considerations in predictive modeling  

This repository contains all required deliverables for the ISOM 835 Individual Term Project.

---

---

## 📊 Dataset Information  

- **Dataset Name:** Predicting Churn for Bank Customers  
- **Creator:** Adammaus  
- **Source:** Kaggle  
- **Link:** https://www.kaggle.com/datasets/adammaus/predicting-churn-for-bank-customers  
- **Rows:** 10,000  
- **Columns:** 14  
- **Target Variable:** `Exited` (1 = churned, 0 = stayed)

### Key Features  
| Feature | Description |
|---------|-------------|
| CreditScore | Customer credit score |
| Geography | Country (France, Spain, Germany) |
| Gender | Male / Female |
| Age | Customer age |
| Tenure | Years with the bank |
| Balance | Account balance |
| NumOfProducts | Number of bank products held |
| HasCrCard | Whether customer has a credit card |
| IsActiveMember | Activity status |
| EstimatedSalary | Annual salary |
| Exited | Churn (target variable) |

---

## 🧪 Google Colab Notebooks  

| Notebook | Description | Link |
|----------|-------------|------|
| **01 – EDA** | Exploratory Data Analysis: distributions, patterns, churn analysis | *(Paste your Colab link here)* |
| **02 – Preprocessing** | Encoding, scaling, train/test split | *(Paste your Colab link here)* |
| **03 – Modeling** | Logistic Regression, Random Forest, evaluation metrics | *(Paste your Colab link here)* |

👉 **To get your Colab link:**  
In Colab → File → Share → Change to “Anyone with the link” → Copy link.

---

## 🧹 Data Preprocessing Summary  

- Removed ID-like fields: `RowNumber`, `CustomerId`, `Surname`  
- One-hot encoded categorical variables (`Gender`, `Geography`)  
- Split data into **80% training / 20% testing** using stratified sampling  
- Standardized numerical features using **StandardScaler**  
- Addressed class imbalance using `class_weight='balanced'` in Random Forest  

---

## 🤖 Machine Learning Models  

### **1. Logistic Regression**  
- Serves as a baseline linear model  
- Works well with scaled data  
- Easy to interpret  

### **2. Random Forest Classifier**  
- Captures non-linear relationships  
- Best-performing model  
- Provides feature importance insights  

---

## 📈 Model Performance Summary  

| Metric | Logistic Regression | Random Forest |
|--------|----------------------|----------------|
| Accuracy | *(insert value)* | *(insert value)* |
| Precision | *(insert value)* | *(insert value)* |
| Recall | *(insert value)* | *(insert value)* |
| F1-Score | *(insert value)* | *(insert value)* |
| AUC | *(insert value)* | *(insert value)* |

### 📌 Conclusion  
**Random Forest outperformed Logistic Regression**, offering:  
- Higher AUC  
- Better recall for churners  
- More stable predictions  

---

## 🔍 Key Findings & Business Insights  

- **Age** is a strong predictor: churn increases for older customers  
- **Germany** has the highest churn rate among geographic categories  
- Customers with **high balance**, **lower tenure**, or **fewer products** show higher churn risk  
- Key actionable strategies:
  - Targeted retention campaigns for at-risk segments  
  - Country-specific customer service improvements  
  - Proactive outreach to older customers  

---

## ⚖️ Ethical Considerations  

- Avoid discriminatory actions based on geography, gender, or age  
- Model predictions must not negatively affect protected groups  
- Customer financial data must remain secure and private  
- Predictions should enable **support and retention**, not punitive measures  
- Human oversight is required during deployment  

---

## 📄 Final Report  

The full 10–12 page project report can be found here:

📄 **Final Report (PDF):** *(Insert link once uploaded)*  
📄 **Word Version:** *(Insert link once uploaded)*  

---

## ▶️ How to Run This Project  

1. Clone or download the repository  
2. Open the notebooks in Google Colab  
3. Install required dependencies  
4. Run each notebook in order:
   - 01_EDA  
   - 02_Preprocessing  
   - 03_Modeling  

---

## 👤 Author  
**Your Name**  
Graduate Student, Suffolk University  
Sawyer Business School  

---

## 🙏 Acknowledgments  
- Dataset provided by Kaggle  
- Python libraries: pandas, numpy, seaborn, scikit-learn  
- ISOM 835 Course Material  
- Instructor: Hasan Arslan  


## 📂 Repository Structure  
