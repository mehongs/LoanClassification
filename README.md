# LoanClassification
## 1. Project Overview
This project utilizes a machine learning algorithm (Logistic Regression) to classify if a person will be 'approved' or 'denied' a loan. The dataset includes 60 rows of data taken from Kaggle.

Given the small sample size of the dataset, this analysis primarily focuses on understanding the core machine learning workflows and exploring data science libraries (such as Pandas and Scikit-Learn).

## 2. Technical Workflow
**Data Preprocessing:** Scanned the dataset for any missing values and used one-hot encoding on categorical values to optimize for Logisitic Regression.

**Subset Separation:** Utilized `train_test_split` to divide the dataset into training and testing subsets with a 80/20 split.

**Model Training:** Fit a binary Logistic Regression model using `scikit-learn` to establish coefficients for each feature.

**Model Prediction:** Created a new, unseen testing subset to be used for prediction.

**Model Validation:** Evaluated performance with Cross Validation, checking for data leakage and imbalanced data.

## 3. Tech Stack
**Language(s):** Python

**Libraries:** Pandas, Scikit-Learn

## 4. Results & Performance
**Accuracy:** 1.0

**Precision/Recall:** 1.0/1.0

**Key Takeaway:** While the algorithm achieved perfect metrics, it is highly unlikely that it is so, most likely due to overfitting and a limited sample size.

## Step 5. Model Validation
The model's robustness was validated using three approaches:
1. Cross validation: Assessed the model's performance stability across multiple data splits to ensure metrics weren't skewed by a lucky train-test split.
2. **Class Imbalance Check:** Evaluated the target variable distribution. While the dataset exhibited class imbalance, this is representative of real-world scenarios and was accounted for during analysis.
3. **Data leakage & feature importance analysis**: The analysis revealed an overwhelming reliance on `credit_score` compared to all other variables. Because the dataset only contains 60 rows, this extreme focus makes overfitting highly likely.
