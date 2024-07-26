# Auditing-of-an-Automated-Decision-System-Loan-Eligibility-Prediction-System

## Overview
This repository contains the capstone project for the course DS-GA 1017 Responsible Data Science, Spring 2024. The project, undertaken by Anna Dominic and Manan Patel, focuses on conducting a technical audit of an Automated Decision System (ADS) designed to predict loan eligibility. The analysis leverages data provided by the Loan Eligible Dataset on Kaggle, and various machine learning models are evaluated for their accuracy, fairness, and robustness.

## Team Members
- Anna Dominic (amd9200@nyu.edu)
- Manan Patel (mp6561@nyu.edu)

## Project Structure

### 1. Background
- **Purpose and Goals**: This ADS integrates machine learning with the traditional loan approval process to enhance efficiency and user experience within the financial sector. It automates the analysis of financial credentials to offer timely predictions of creditworthiness and repayment likelihood.
- **Trade-offs**: The ADS balances speed vs. accuracy, automation vs. personalized assessment, and overall accuracy vs. fairness.

### 2. Input and Output
- **Data Description**: The dataset contains personal information, employment details, financial metrics, loan specifics, credit history, and geographical data.
- **Input Features**: Includes variables such as Loan_ID, Gender, Married status, Dependents, Education, Self_Employed status, ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, and Credit_History.
- **Data Preparation and Preprocessing**: Three versions of the data preparation process were evaluated:
  - **Original Implementation**: Identified key errors in preprocessing steps.
  - **With Imputation Implementation**: Retained mean and mode imputation while rectifying errors.
  - **Without Imputation Implementation**: Removed rows with missing values instead of imputing them.

### 3. Implementation and Validation
- **Data Cleaning and Pre-processing**: Addressed missing values, outlier removal, skewed distribution treatment, and data scaling.
- **Implementation Overview**: Chose Random Forest as the primary algorithm for loan approval prediction.
- **Validation of the ADS**: Used holdout validation and cross-validation to assess model performance.

### 4. Outcome
- **Auditing Methodology**: Utilized tools like Fairlearn, Aequitas, and SHAP to audit the ADS for fairness and transparency.
- **Overall Metrics**: Compared the performance of different preprocessing implementations using metrics such as accuracy, precision, recall, selection rate, false positive rate, and false negative rate.
- **SubGroup Analysis**: Evaluated the ADS's performance across different demographic subgroups.

### 5. Summary
- **Data Appropriateness**: The dataset was appropriate but required careful preprocessing to ensure data quality.
- **Implementation Robustness, Accuracy, and Fairness**: The Random Forest classifier demonstrated high accuracy and balanced performance, with some biases noted in gender and marital status categories.
- **Deployment Considerations**: While the model is robust, further refinement is needed to address observed biases.
- **Recommendations for Improvement**: Suggested enhancements in data collection, processing, and model analysis to improve fairness and accuracy.
- **Conclusion**: The ADS shows strong potential for effective loan eligibility prediction, with targeted refinements needed to ensure fairness and equity.

### 6. Appendix
Includes detailed exploratory data analysis, data preprocessing steps, and additional visualizations supporting the project findings.

## Files
- **Project Report**: Detailed report of the project findings (PDF)
- **Notebooks**: Jupyter notebooks used for exploratory data analysis (EDA), original implementation, various machine learning models, and fairlearn audit.
- **Data**: Loan Eligible Dataset from Kaggle (linked due to large size)

## Acknowledgements
We would like to thank the instructors and teaching assistants of DS-GA 1017 Responsible Data Science for their guidance and support throughout this project. Additionally, we acknowledge Kaggle for providing the dataset used in this analysis.


