# Loan Prediction using Logistic Regression

## 📌 Project Overview
This project predicts whether a loan applicant is eligible or not using Logistic Regression. The model is trained on historical data of applicants, considering factors like income, credit history, loan amount, and more.

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

## 🚀 How to Run
1. Clone this repository:  
