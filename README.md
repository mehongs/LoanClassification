# LoanClassification
## 1. Project Overview
This project utilizes a machine learning algorithm (Logistic Regression) to classify if a person will be 'approved' or 'denied' a loan. The dataset includes 60 rows of data taken from Kaggle.

Given the small sample size of the dataset, this analysis primarily focuses on understanding the core machine learning workflows and exploring data science libraries (such as Pandas and Scikit-Learn).

## 2. Technical Workflow
**Data Preprocessing:** Scanned the dataset for any missing values and used one-hot encoding on categorical values to optimize for Logisitic Regression.
**Subset Separation:** Utilized 'train_test_split' to divide the dataset into training and testing subsets with a 80/20 split.
**Nodel Training:** Fit a binary Logistic Regression model using 'scikit-learn' to establish coefficients for each feature.
**Model Prediction:** Created a new, unseen testing subset to be used for prediction.
**Model Validation:** Evaluated performance with Cross Validation, checking for data leakage and imbalanced data.

## 3. Tech Stack
**Languages:** Python
**Libraries:**

## 4. Resuls & Performance
**Accuracy:** 1.0
**Precision/Recall:** 1.0
**Key Takeaway:** 
