# Bank Customer Churn Analysis & Prediction

## Project Overview
Banks lose revenue when customers close their accounts — this is called *customer churn*.  
This project simulates a real-world data analyst workflow to identify reasons for churn and predict at-risk customers.

*Key Goals:*
- Understand patterns in customer churn
- Build predictive models to identify at-risk customers
- Provide actionable insights to improve customer retention

## Dataset
- Contains bank customer information: age, balance, credit score, geography, account activity
- Columns include: CustomerId, CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary, Exited (target)
- Source: Simulated dataset for educational purposes

## Project Workflow

### 1. Data Preparation
- Loaded raw dataset from data/raw/
- Checked data types, missing values, and target distribution
- Split the dataset into *train (80%)* and *test (20%)* sets and saved in data/processed/:
  - train_processed.csv  
  - test_processed.csv  

### 2. Exploratory Data Analysis (EDA)
- Visualized distributions of numeric and categorical variables
- Checked correlations between features and target
- Insights discovered:
  - Higher balances and lower credit scores linked to higher churn
  - Age and tenure showed patterns in churn probability
- Created charts for GitHub/LinkedIn:
  - Histograms, boxplots, heatmaps, correlation matrices

### 3. Model Building
- *Baseline Model:* Logistic Regression  
  - Evaluated with Accuracy, Precision, Recall, F1 Score, and ROC-AUC
- *Advanced Model:* Random Forest Classifier  
  - Captured nonlinear patterns, outperformed Logistic Regression
  - Plotted *top 10 feature importance* for readability

*Top Features:*  
- Balance  
- CreditScore  
- Age  
- Tenure  
- IsActiveMember

### 4. Model Evaluation
| Model | Accuracy | Precision | Recall | F1 Score | ROC AUC |
|-------|---------|-----------|--------|----------|---------|
| Logistic Regression | 0.81 | 0.68 | 0.52 | 0.59 | 0.85 |
| Random Forest | 0.87 | 0.76 | 0.63 | 0.69 | 0.92 |

Replace metrics with your actual results

- Random Forest showed better overall performance
- Confusion matrices and feature importance charts used for insights

### 5. Model Saving
- Trained Random Forest model saved locally as models/rf_churn_model.pkl
- *Not uploaded to GitHub* due to file size limits; available upon request
