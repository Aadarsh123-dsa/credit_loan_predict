# credit_loan_predict
# PROBLEM_STATEMENT
A mid-sized financial company named SecureTrustBank offers personal and home loans to customers across urban and rural regions of India. Every day, hundreds of customers apply for loans through online and branch applications.
Until now, SecureTrust Bank has been using a manual verification process where loan officers evaluate applications by checking income proofs, employment details, credit history, and other documents. This process is time-consuming, biased & inconsistent.
As a result, the bank faces two major challenges:
1. leading to loss of business.
2. Good customers sometimes get rejected.
   
To solve this problem, the bank wants to introduce an intelligent loan approval system powered by Machine Learning that can automatically analyse applicant details and predict whether a loan should be Approved or Rejected before final human verification.
You are hired as a Machine Learning Engineer to design and develop this intelligent system using historical loan application data. The system must learn hidden patterns from previous customer records and provide accurate, fast, and unbiased loan approval decisions.
# Dataset Description
Each row in the dataset represents a loan applicant and contains multiple attributes describing their personal, financial, and credit information.
## 📊 Dataset Description

| Column               | Description                                      |
|---------------------|--------------------------------------------------|
| Applicant_ID        | Unique applicant ID                              |
| Applicant_Income    | Monthly income of applicant                      |
| Coapplicant_Income  | Monthly income of co-applicant                   |
| Employment_Status   | Salaried / Self-Employed / Business              |
| Age                 | Applicant age                                    |
| Marital_Status      | Married / Single                                 |
| Dependents          | Number of dependents                             |
| Credit_Score        | Credit bureau score                              |
| Existing_Loans      | Number of already running loans                  |
| DTI_Ratio          | Debt-to-Income ratio                             |
| Savings             | Savings balance                                 |
| Collateral_Value    | Value of collateral provided                     |
| Loan_Amount         | Loan amount requested                            |
| Loan_Term           | Loan duration (months)                           |
| Loan_Purpose        | Home / Education / Personal / Business           |
| Property_Area       | Urban / Semi-Urban / Rural                       |
| Education_Level     | Graduate / Postgraduate / Undergraduate          |
| Gender              | Male / Female                                    |
| Employer_Category   | Govt / Private / Self                            |
| Loan_Approved       | 1 = Approved, 0 = Rejected                       |
## Dataset Source 
The dataset used in this project is a synthetic dataset created and modified for educational purposes to simulate real-world loan approval scenarios.
The dataset is included in this repository as `loan_approval_data.csv`.
## Exploratory data analysis 
1.“Applicants with higher income show a slightly greater likelihood of loan approval; however, the overlap between approved and rejected groups suggests that income alone is not a strong deciding factor.”
2. “Credit score shows a strong positive relationship with loan approval, with approved applicants having significantly higher median scores. This indicates that credit score is a key predictor of loan eligibility.”
3. “Applicants with higher debt-to-income ratios are more likely to be rejected, indicating that higher financial burden negatively impacts loan approval decisions.”
4. “Savings show a moderate influence on loan approval, but the significant overlap suggests it is not a dominant factor compared to credit score or DTI ratio.”
5. “Among the analyzed features, Credit Score and DTI Ratio demonstrate the strongest relationship with loan approval, making them critical predictors. In contrast, Applicant Income and Savings show weaker individual influence, indicating that loan approval decisions are driven more by credit risk and financial stability than income alone.”
6. “Categorical feature analysis indicates that property area has a noticeable influence on loan approval decisions, with urban applicants showing higher approval tendencies. In contrast, marital status exhibits only a mild impact, suggesting that financial factors may play a more dominant role than demographic attributes.”
7. The correlation matrix was analyzed to understand relationships between features and the target variable (Loan_Approved). It was observed that Credit_Score has the highest positive correlation (0.45), indicating it is a strong predictor. Income-related features also showed moderate correlation, while most other variables had weak relationships.This suggests that while some features strongly influence the outcome, others may contribute less and require model-based evaluation.The insights from correlation analysis guided feature selection for model training.
