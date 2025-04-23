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


## Loan Eligibility Prediction - Model Performance

After training the Logistic Regression model, we evaluated its performance using key metrics:

### 📊 Model Evaluation Metrics:
- **Accuracy**: `0.76`
- **Precision**: `0.75`
- **Recall**: `0.95`
- **F1 Score**: `0.84`
- **Confusion Matrix**:
- `[[18 25]
 [ 4 76]]`


### 📌 Interpretation:
- **Accuracy**: Measures how often the model correctly predicts loan eligibility.
- **Precision**: Out of the predicted eligible loans, how many were actually eligible?
- **Recall**: Out of all actual eligible loans, how many did the model identify?
- **F1 Score**: A balance between precision and recall.

Higher values for precision, recall, and F1-score indicate a better-performing model.

---

### 🚀 Next Steps:
- **Feature Engineering**: Improve the model by adding or transforming features.
- **Hyperparameter Tuning**: Try adjusting parameters like regularization (`C` in `LogisticRegression`).
- **Model Comparison**: Experiment with Decision Trees or Random Forests for better performance.


---
🔍 **Developed by Surekha Thombare**


