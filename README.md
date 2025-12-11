# 🏦 Bank Customer Churn Prediction  
### ISOM 835 – Individual Term Project  
Instructor: Hasan Arslan  

## 📌 Project Overview
This project applies predictive analytics and machine learning to identify customers who are likely to leave a bank (churn). Early identification of at-risk customers allows the bank to design effective retention strategies and reduce revenue loss.

I used the Bank Customer Churn dataset from Kaggle, explored key patterns through EDA, prepared the data through preprocessing, and built two machine learning models: Logistic Regression and Random Forest. The final analysis includes model evaluation, feature importance, business insights, and ethical considerations.

---

## 📂 Repository Structure
├── notebooks/
│ └── Bank_Customer_Churn_Analysis.ipynb
├── visuals/
│ └── plots, charts, heatmaps
├── reports/
│ └── Final_Report.pdf
│ └── Final_Report.docx
└── README.md

---

## 📊 Dataset
- Source: Kaggle  
  https://www.kaggle.com/datasets/adammaus/predicting-churn-for-bank-customers  
- Rows: 10,000  
- Target variable: **Exited** (1 = churned, 0 = stayed)

---

## 🧪 Methods Used
- Exploratory Data Analysis (EDA)  
- One-Hot Encoding  
- Train/Test split with stratification  
- Feature Scaling (StandardScaler)  
- Logistic Regression  
- Random Forest Classifier  
- Evaluation: Accuracy, Precision, Recall, F1-score, Confusion Matrix, ROC Curve  
- Feature Importance Analysis  

---

## 🚀 Key Findings
- Customers in Germany have a higher churn rate.
- Older customers are more likely to churn.
- Inactive members churn more frequently.
- Customers with higher balances still churn, signaling deeper service issues.
- Random Forest outperforms Logistic Regression in prediction quality.

---

## 🧠 Business Insights
- Engage inactive customers through targeted outreach.
- Develop retention programs for older customers.
- Review service experience for German customers specifically.
- Re-evaluate product bundles for clarity and customer satisfaction.
- Prioritize high-balance customers for proactive retention.

---

## ⚖ Ethical Considerations
I avoided using sensitive attributes unfairly and ensured that model decisions do not promote discrimination. Churn predictions should be used to improve customer experience—not to deny services. I also considered privacy, transparency, and responsible model interpretation.

---

## 📘 How to Run the Notebook
1. Open the notebook in Google Colab  
2. Upload **Churn_Modelling.csv**  
3. Run all cells in order  

---

## 👤 Author
**Samuel Quartey**  
ISOM 835 – Predictive Analytics & Machine Learning  
Suffolk University  

---

## 📄 License
For academic use only.
