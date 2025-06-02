# Customer-Churn-Prediction
Telco Customer Churn Prediction using Python's SKLearn

1. **Project Title**
Telco Customer Churn Prediction using SKLearn Library

2. **Project Description**
This project analyzes the Telco Customer Churn dataset to identify key factors that influence customer attrition and to build a predictive model that can help telecom companies reduce churn and improve customer retention.

3. **Dataset Information**
Kaggle Telco Customer Churn Dataset

Key features: 'customerID', 'gender', 'SeniorCitizen', 'Partner', 'Dependents',
       'tenure', 'PhoneService', 'MultipleLines', 'InternetService',
       'OnlineSecurity', 'OnlineBackup', 'DeviceProtection', 'TechSupport',
       'StreamingTV', 'StreamingMovies', 'Contract', 'PaperlessBilling',
       'PaymentMethod', 'MonthlyCharges', 'TotalCharges'

Target variable: Churn

4. **Exploratory Data Analysis (EDA)**

Distribution of churn vs non-churn customers using Histogram
Correlation heatmap
Comparison of numerical and categorical features using countplots
Key findings: (short tenure and month-to-month contracts are associated with high churn)

5.  **Data Preprocessing**
Replaced blank values in the TotalCharges column with 0 because those rows were important and 0 was a reasonable substitution.
No other missing values were found.
Converted categorical features to numeric using Label Encoding.
Since numerical features were not normally distributed, focused on tree-based models that don’t require normality assumptions.
Applied SMOTE on the training data to balance the churn classes.

6.  **Model Building**
List of models used:

DecisionTree
Random Forest
XGBoost 

7. **Evaluation Metrics**

confusion_matrix,
classification_report,
accuracy_score

RandomForest Classifier model performed best with **84% cross val score** hence trained the data with the RF model.

8. **Tools & Technologies**
Libraries used:
Python, pandas, NumPy, scikit-learn, seaborn, matplotlib

Models used: 
XGBoost, Decision Tree, Random Forest

**Notebook used:**
Jupyter Notebook
Kaggle, GitHub (if applicable)

9. **Future Work**
Ideas for improvements:

Use deep learning models
Deploy with Streamlit or Flask
Integrate customer lifetime value (CLV) prediction
Automate model updates with new data

10.  **Author or Credits**
Rashmi Krishnamohan (https://www.linkedin.com/in/rashmi-krishnamohan/) 
