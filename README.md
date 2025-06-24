# Telecom Customer Churn Prediction

## Overview
This project analyzes and predicts customer churn for a telecom company using real-world data. Customer churn refers to customers leaving a company's services. Reducing churn is crucial for telecom businesses, as acquiring new customers is often more expensive than retaining existing ones.

## Data Source
- **Kaggle IMB Telecom Churn Dataset**
- [Kaggle Dataset Link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

## Business Context
Telecom companies offer a variety of services such as phone, internet, and streaming. Understanding why customers leave helps companies:
- Improve customer satisfaction
- Develop targeted retention strategies
- Increase profitability by reducing churn rates

## Project Objectives
- Explore and visualize the data to identify patterns and trends
- Preprocess and prepare the data for modeling
- Build and evaluate machine learning models to predict customer churn
- Identify key factors that influence churn
- Provide actionable insights for business decision-making

## Methodology
This project follows the **CRISP-DM** (Cross-Industry Standard Process for Data Mining) methodology:
1. **Business Understanding**: Define project objectives and requirements from a business perspective.
2. **Data Understanding**: Collect, describe, and explore the data.
3. **Data Preparation**: Clean, transform, and prepare data for modeling.
4. **Modeling**: Apply machine learning algorithms and build predictive models.
5. **Evaluation**: Assess model performance and validate results.
6. **Deployment/Next Steps**: (Optional) Plan for model deployment or further actions.

## Data Description
The dataset contains detailed information about each customer, including:
- **Churn**: Whether the customer left in the last month (target variable)
- **Services Signed Up**: Phone, multiple lines, internet, online security, online backup, device protection, tech support, streaming TV, and streaming movies
- **Account Information**: Tenure, contract type, payment method, paperless billing, monthly charges, and total charges
- **Demographics**: Gender, age range, partner status, and dependents

## Notebooks & Scripts
- `Telecom_Charn_Prediction.ipynb`: Main notebook containing all data exploration, preprocessing, modeling, and evaluation steps.
- `Data/`: Contains raw and processed datasets used in the project.

## Key Steps
1. **Data Exploration**: Visualize distributions, check for missing values, and understand feature relationships.
2. **Data Cleaning & Preprocessing**: Handle missing values, encode categorical variables, and scale features.
3. **Feature Engineering**: Apply PCA and LDA for dimensionality reduction.
4. **Modeling**: Train and evaluate Logistic Regression, Random Forest, XGBoost, and SVM models on original and transformed features.
5. **Evaluation**: Compare models using accuracy and F1 score, and summarize results in a report.

## Results Summary
- The best-performing models and feature sets are highlighted in the notebook.
- Key factors influencing churn include tenure, monthly charges, and contract type.
- Actionable insights are provided for business decision-making.

## How to Run
1. Clone the repository:
   ```
   git clone https://github.com/irtezachy/Telecom-Churn-Data-Prediction.git
   ```
2. Install required Python packages (see notebook for details).
3. Open and run the notebook `Telecom_Charn_Prediction.ipynb` in Jupyter or VS Code.

## License
This project is for educational and research purposes. Data is provided by Kaggle IMB.

---

# Project Report

## Introduction
Customer churn is a major concern for telecom companies. This project uses the Kaggle IMB dataset to analyze churn patterns and build predictive models to identify at-risk customers.

## Data Preparation
- Loaded and explored the dataset for missing values and data types.
- Cleaned data by handling missing values and encoding categorical variables.
- Scaled numerical features and applied dimensionality reduction (PCA, LDA).

## Modeling
- Trained Logistic Regression, Random Forest, XGBoost, and SVM models.
- Evaluated models on original, PCA, and LDA-transformed features.
- Compared performance using accuracy and F1 score.

## Key Findings
- **Tenure**: Customers with short tenure are more likely to churn.
- **Monthly Charges**: Higher monthly charges are associated with higher churn rates.
- **Contract Type**: Month-to-month contracts have higher churn compared to longer-term contracts.
- **Feature Engineering**: Dimensionality reduction (PCA, LDA) can improve model performance in some cases.

## Recommendations
- Target customers with short tenure and high monthly charges for retention campaigns.
- Offer incentives for customers on month-to-month contracts to switch to longer-term plans.
- Monitor key features identified by the models to proactively address churn risk.

## Conclusion
This project demonstrates a full data science workflow for churn prediction, from data exploration to actionable business insights. The approach can be adapted to other customer retention problems in telecom and beyond.
