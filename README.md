Holistic Data Preparer

Project Overview
Holistic Data Preparer is a comprehensive data preprocessing and feature engineering project designed to prepare raw customer credit data for machine learning modeling. The goal of this project is to transform unstructured and inconsistent data into a clean, structured, and model-ready dataset for predicting loan default risk.

This project simulates a real-world scenario where a data scientist works with multi-source data and applies end-to-end preprocessing techniques.

Objective
The main objective of this project is to:
- Perform complete data preprocessing
- Handle missing values using multiple techniques
- Detect and treat outliers
- Encode categorical and numerical features
- Apply data transformations and scaling
- Engineer new meaningful features
- Prepare a final dataset suitable for machine learning

Dataset Description
The dataset represents customer credit risk data and includes the following:

Demographic Data
- Age
- Gender
- Region
- Education Level
- Employment Type

Financial Data
- Annual Income
- Loan Amount
- Loan Purpose
- Credit Score
- Repayment History

Behavioral Data
- Transaction Count
- Spending Ratio

Date Feature
- Join Date

Target Variable
- Default Flag (0 = No Default, 1 = Default)

Data Sources
Data is collected from multiple sources:
- CSV file for main dataset
- JSON file for customer metadata
- SQL database for repayment history
- API for external data

Project Workflow

1. Data Acquisition
Data is loaded from CSV, JSON, SQL, and API sources and merged into a unified dataset.

2. Data Understanding
Basic analysis is performed using info, describe, and profiling reports to understand data distribution and quality.

3. Data Cleaning
- Missing values handled using multiple techniques
- Duplicate records checked and removed
- Data types corrected

4. Missing Value Handling
- Mean and median imputation for numerical data
- Most frequent imputation for categorical data
- Random sampling and missing indicators
- Advanced methods such as KNN and MICE

5. Outlier Handling
- Z Score Method
- IQR Method
- Percentile Method
- Winsorization

6. Feature Engineering
- Date feature extraction (year, month, day, weekday)
- Creation of new features:
  - Debt-to-Income Ratio
  - Average Monthly Transactions
  - Spending-to-Income Ratio

7. Encoding
- Ordinal encoding for education level
- Label encoding for gender
- One-hot encoding for region and loan purpose

8. Numerical Encoding
- Binning
- Binarization
- Quantile binning
- K-Means binning

9. Feature Scaling
- Standardization
- Normalization
- Min-Max scaling
- MaxAbs scaling
- Robust scaling

10. Data Transformation
- Log transformation
- Square root transformation
- Reciprocal transformation
- Power transformation (Yeo-Johnson)

11. Column Transformer
Used to apply different preprocessing techniques to different columns in a pipeline.

Final Output
The final dataset is:
- Cleaned and consistent
- Free from missing values
- Outliers handled properly
- Encoded and scaled
- Ready for machine learning

Output File
final_cleaned_dataset.csv

Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- SciPy
- SQLite
- Requests
- ydata-profiling

Key Learnings
- End-to-end data preprocessing pipeline
- Handling real-world messy datasets
- Feature engineering techniques
- Importance of scaling and transformation
- Working with multiple data sources

Conclusion
This project demonstrates a complete workflow for preparing raw data for machine learning. By applying various preprocessing and feature engineering techniques, the dataset is transformed into a high-quality input suitable for predictive modeling.
