# Loan-Approval-Prediction 🚀

## 📌 Project Overview  
Loan providers face challenges in manually assessing loan applications, which can lead to delays and inconsistencies. The objective of this project is to develop a machine learning model that automates the loan approval process by analyzing historical data, thereby improving efficiency and accuracy.

## 📂 Dataset  
- **Source**: The dataset consists of 614 records with 13 features.  
- **Key Features**:  
  - `ApplicantIncome` - Monthly income of the applicant  
  - `CoapplicantIncome` - Monthly income of the co-applicant  
  - `LoanAmount` - Loan amount requested  
  - `Credit_History` - Whether the applicant has a good credit history (1 = Yes, 0 = No)  
  - `Loan_Status` (Target) - Whether the loan was approved (`Y` or `N`)  

## ⚙️ Data Preprocessing  
- **Handling Missing Values**: Mode/median imputation  
- **Feature Scaling**: StandardScaler applied for normalization  
- **Handling Imbalanced Data**: SMOTE (Synthetic Minority Oversampling Technique)  
- **Encoding**: Label Encoding for categorical variables  

## 🔍 Exploratory Data Analysis (EDA)  
- Visualized data distributions, correlations, and outliers  
- Used boxplots and histograms to analyze feature distributions  
- Detected and treated skewness using log transformation  

## 📊 Models Used  
1. **Logistic Regression**  
2. **Random Forest**  
3. **AdaBoost (Best Model)**  

## 🏆 Model Comparison  
| Model               |  Training Accuracy |  Testing Accuracy  |     Observations     |
|---------------------|--------------------|--------------------|----------------------|
| Logistic Regression | 78.66%             | 78.69%             | Baseline model       |
| Random Forest       | 100%               | 83.24%             | Overfitting detected |
| AdaBoost (Best)     | 82.27%             | 83.43%             | Balanced performance |

## 📌 Key Takeaways  
✅ Credit history & property play a significant role in loan approval  
✅ Random Forest overfits, while AdaBoost generalizes well  
✅ Feature scaling and balancing techniques improve model performance  

## 🚀 Future Improvements  
- **Hyperparameter tuning** for AdaBoost to further optimize performance  
- **More features** like employment length and debt-to-income ratio  
- **Deploying the model** using Flask or Streamlit  

## 📌 Technologies Used
* Python 🐍 (Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn)
* Jupyter Notebook 
* Machine Learning Algorithms
