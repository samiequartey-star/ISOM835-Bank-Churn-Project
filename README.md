# ISOM835-Bank-Churn-Project
Customer Churn Prediction
Project Overview
This project aims to build and evaluate machine learning models to predict customer churn for a bank. Customer churn is a critical problem for businesses as retaining existing customers is often more cost-effective than acquiring new ones. By identifying customers at risk of churning, the bank can implement targeted retention strategies.

Dataset
The dataset used for this analysis is Churn_Modelling.csv, which contains 10,000 entries and 14 features related to bank customers, including demographics, financial details, and churn status.

Exploratory Data Analysis (EDA) Summary
Key Findings:
Data Quality: The dataset is clean with no missing values.
Target Variable Imbalance: Approximately 20.37% of customers have churned (Exited=1), indicating a significant class imbalance that needs to be addressed during modeling.
Numerical Feature Distributions:
CreditScore is relatively normally distributed.
Age is right-skewed, with most customers in their 30s and 40s.
Balance is heavily skewed, with a large proportion of customers having a zero balance.
EstimatedSalary and Tenure show fairly uniform distributions.
Categorical Feature Distributions:
Geography is dominated by France (50.14%).
Gender has slightly more males (54.57%) than females.
Most customers have 1 or 2 products (50.84% and 45.90% respectively).
A large majority (70.55%) of customers possess a credit card.
IsActiveMember is fairly balanced (51.51% active).
Correlations with Churn (Exited):
Age shows the strongest positive correlation with Exited (0.29), suggesting older customers are more likely to churn.
Balance has a notable positive correlation with Exited (0.12).
IsActiveMember is negatively correlated with Exited (-0.16), indicating active members are less likely to churn.
Data Preprocessing and Feature Engineering
The following steps were performed to prepare the data for machine learning models:

Handling Missing Values: No missing values were found, so no action was required.
Addressing Outliers: Outliers in Age and Balance were identified using the IQR method and capped at their respective upper IQR bounds.
Encoding Categorical Variables: Geography and Gender were One-Hot Encoded. Other categorical-like features (HasCrCard, IsActiveMember, NumOfProducts) were retained in their original numerical format.
Scaling Numerical Features: CreditScore, Age, Tenure, Balance, NumOfProducts, and EstimatedSalary were scaled using StandardScaler to ensure uniform contribution to model training.
Feature Engineering: A new binary feature, HasBalance, was created to explicitly capture whether a customer had an account balance greater than zero.
Train/Test Split: The preprocessed dataset was split into 80% training and 20% testing sets using stratified sampling on the Exited variable to maintain class distribution.
Model Development and Evaluation
Two different machine learning models, Logistic Regression and Random Forest, were implemented and evaluated for customer churn prediction. Hyperparameter tuning was performed using GridSearchCV with cross-validation to optimize their performance.

Initial Model Performance:
Logistic Regression: Accuracy: 0.8155, Precision: 0.6284, Recall: 0.2285, F1-Score: 0.3351, ROC AUC: 0.7845
Random Forest: Accuracy: 0.8665, Precision: 0.7966, Recall: 0.4619, F1-Score: 0.5848, ROC AUC: 0.8512
Hyperparameter Tuning Results:
Logistic Regression: Best Parameters: {'C': 0.01, 'solver': 'lbfgs'}, Best CV ROC AUC: 0.772
Random Forest: Best Parameters: {'max_depth': 10, 'max_features': 'sqrt', 'n_estimators': 300}, Best CV ROC AUC: 0.8627
Tuned Model Comparison:
Metric	Tuned Logistic Regression	Tuned Random Forest
Accuracy	0.8105	0.8675
Precision	0.6400	0.8349
Recall	0.1572	0.4349
F1-Score	0.2525	0.5719
ROC AUC Score	0.7833	0.8663
Conclusion:
The Random Forest model consistently outperformed the Logistic Regression model across all key evaluation metrics, both in its initial and hyperparameter-tuned versions. This makes Random Forest the more effective model for predicting customer churn in this dataset. The tuned Random Forest achieved an accuracy of 0.8675 and an ROC AUC of 0.8663, demonstrating good predictive capability.

Future Work
Further optimization could explore advanced ensemble techniques or different class balancing strategies (e.g., SMOTE) to potentially improve recall without significantly sacrificing precision.
Investigate feature importances from the Random Forest model to gain deeper insights into the primary drivers of churn.
Consider alternative models such as Gradient Boosting (e.g., XGBoost, LightGBM) for potentially higher performance.
Conduct more in-depth segment analysis to develop highly targeted retention programs based on specific customer characteristics.

## 📄 Final Report  

The full 10–12 page project report can be found here:

📄 **Final Report (PDF):** *(Insert link once uploaded)*  
📄 **Word Version:** *(Insert link once uploaded)*  

---

## ▶️ How to Run This Project  

1. Download the repository  
2. Open the notebooks in Google Colab  
3. Install required dependencies  
4. Run each notebook in order:
   - 01_EDA  
   - 02_Preprocessing  
   - 03_Modeling  

---

## 👤 Author  
Samuel Quartey
Graduate Student, Suffolk University  
Sawyer Business School  

---

## 🙏 Acknowledgments  
- Dataset provided by Kaggle  
- Python libraries: pandas, numpy, seaborn, scikit-learn  
- ISOM 835 Course Material  
- Instructor: Hasan Arslan  


## 📂 Repository Structure  
