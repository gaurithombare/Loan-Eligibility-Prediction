# Loan Eligibility Prediction using Machine Learning




## 📚 Table of Contents
- [Project Overview](#-project-overview)
- [Dataset](#-dataset)
- [Methodology](#️-methodology)
- [Model Evaluation](#loan-eligibility-prediction---model-performance)
- [Model Performance Summary](#-model-performance-summary)
- [Model Analysis](#-model-analysis)
- [Interpretation](#-interpretation)
- [Next Steps](#-next-steps)


## 📌 Project Overview
This project predicts whether a loan applicant is eligible or not using various machine learning models including Logistic Regression, Decision Tree, and Random Forest. Models are evaluated based on accuracy, recall, precision, and F1-score.




## 📊 Dataset
- **Source:** The dataset is provided in this repository under the `data` folder.
- **Filename:** `train.csv`
- **Features:**  
  - `Loan_ID` – Unique identifier for each loan  
  - `Gender` – Male/Female  
  - `Married` – Marital status (Yes/No)  
  - `Dependents` – Number of dependents  
  - `Education` – Education level (Graduate/Not Graduate)  
  - `Self_Employed` – Employment status (Yes/No)  
  - `ApplicantIncome` – Income of the applicant  
  - `CoapplicantIncome` – Income of the co-applicant  
  - `LoanAmount` – Loan amount applied for  
  - `Loan_Amount_Term` – Term of the loan (in months)  
  - `Credit_History` – Credit history (1 = good, 0 = bad)  
  - `Property_Area` – Property location (Urban/Rural/Semiurban)  
  - `Loan_Status` – Loan approval status (Y/N)  

- **Target Variable:**  
  - `Loan_Status` (Y = Approved, N = Not Approved)  

- **How to Use:**  
  - The dataset is already included in this repository.  
  - No need to download separately; just load `train.csv` in the notebook.  

## 🛠️ Methodology
1. **Data Preprocessing** - Handling missing values, encoding categorical variables, scaling numerical data.  
2. **Exploratory Data Analysis (EDA)** - Visualizing key insights using Matplotlib and Seaborn.  
3. **Feature Engineering** - Selecting the most relevant features to improve model performance.  
4. **Model Training** - Implementing Logistic Regression using Scikit-Learn.  
5. **Evaluation Metrics** - Assessing performance using Accuracy, Precision, Recall, F1-score, and Confusion Matrix.  


## Loan Eligibility Prediction - Model Performance

After training the Logistic Regression model, we evaluated its performance using key metrics:






## 📊 Model Performance Summary

| Model                | Accuracy | Precision | Recall | F1 Score | Confusion Matrix         |
|----------------------|----------|-----------|--------|----------|--------------------------|
| Logistic Regression  | 0.76     | 0.75      | 0.95   | 0.84     | [[18, 25], [4, 76]]      |
| Decision Tree        | 0.789    | 0.76      | 0.99   | 0.86     | [[18, 25], [1, 79]]      |
| Random Forest        | 0.789    | 0.76      | 0.99   | 0.86     | [[18, 25], [1, 79]]      |



## 🔍 Model Analysis

### 🎯 Logistic Regression:
- **High recall (0.95)**: It correctly catches most approved loans.
- But **25 false positives**, meaning it's approving many that should have been denied.
- Might be **underfitting** a bit (due to the linear nature of the model).

---

### 🌳 Decision Tree & 🌲 Random Forest:
- **Much better recall (0.9875)** and **lower false negatives (only 1)**.
- Slightly better **accuracy** and **F1 score** than Logistic Regression.
- **Same confusion matrix** — Random Forest and Decision Tree may be acting similarly due to **shallow tree depth** or **small dataset size**.





### 📌 Interpretation:
- **Accuracy**: Measures how often the model correctly predicts loan eligibility.
- **Precision**: Out of the predicted eligible loans, how many were actually eligible?
- **Recall**: Out of all actual eligible loans, how many did the model identify?
- **F1 Score**: A balance between precision and recall.

Higher values for precision, recall, and F1-score indicate a better-performing model.

---






### 🚀 Next Steps:
- **Feature Engineering**: Further improve model performance by creating features like total income, income-to-loan ratio, or interaction terms.
- **Hyperparameter Tuning**: Use techniques like GridSearchCV or RandomizedSearchCV to tune model parameters (e.g., `max_depth`, `n_estimators`, or `C` for Logistic Regression).
- **Model Deployment**: Deploy the final Random Forest model using Streamlit, Flask, or any other tool to create a user interface.
- **Cross-Validation**: Use k-fold cross-validation to ensure model generalization and avoid overfitting.

---
> ✅ Final Model Used: **Random Forest Classifier**


---
🔍 **Developed by Surekha Thombare**


