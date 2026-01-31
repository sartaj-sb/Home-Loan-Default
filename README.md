🏦 Home Loan Default Prediction (PRCP-1006)
📌 Project Overview

This project aims to predict whether a home loan applicant is likely to default using historical loan and applicant data.
The goal is to assist financial institutions in risk assessment and decision-making by identifying high-risk applicants before loan approval.

The notebook implements a complete classification pipeline, covering:

Exploratory Data Analysis (EDA)

Data preprocessing

Model training and evaluation

Business interpretation of results

🎯 Problem Statement

Loan defaults pose significant financial risk to banks and lending institutions.
By leveraging applicant and loan-related features, this project attempts to:

classify applicants as defaulters or non-defaulters

understand key factors contributing to default risk

support data-driven lending decisions

📊 Dataset

Dataset: Home Loan / Credit Default Dataset

Target Variable: Loan default status

Feature Types:

Applicant demographics

Income-related attributes

Loan characteristics

Credit history indicators

Key Observations

Dataset contains both numerical and categorical features

Class imbalance is present between defaulters and non-defaulters

Some features contain missing or inconsistent values requiring preprocessing

🔍 Exploratory Data Analysis (EDA)
Target Distribution

Majority of applicants are non-defaulters

Minority class (defaulters) represents higher business risk

Class imbalance impacts model evaluation and metric selection

Feature Insights

Credit history is a strong indicator of loan repayment behavior

Applicant income and loan amount influence default probability

Certain categorical features show distinct default patterns

Correlation Analysis

Some financial variables show moderate correlation

Multicollinearity considered during model interpretation

🛠️ Data Preprocessing & Feature Engineering

Handled missing values appropriately for numerical and categorical features

Encoded categorical variables into numerical representations

Removed or corrected inconsistent data entries

Split data into training and testing sets

Ensured no target leakage during preprocessing

🤖 Modeling Approach
Models Used

Classification models were trained to predict loan default and evaluated using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

Model Evaluation

Recall for defaulters was emphasized due to business importance

Trade-off between false positives and false negatives was analyzed

Final model selected based on balanced performance rather than accuracy alone

📈 Model Interpretation
Key Risk Indicators Identified

Credit history

Applicant income

Loan amount

Employment and dependents-related features

These factors significantly influence the probability of loan default and align with real-world lending logic.

💡 Business Insights

Credit history is the strongest predictor
Applicants with poor credit history are far more likely to default.

Income-to-loan relationship matters
Higher loan amounts relative to income increase default risk.

Risk-aware decision-making is essential
False negatives (predicting non-default for defaulters) are costlier than false positives.

Model should support, not replace, human judgment
Predictions can be used as a screening tool rather than a final decision-maker.

⚠️ Challenges Faced

Class imbalance in the target variable

Encoding multiple categorical features

Choosing appropriate evaluation metrics for a risk-sensitive problem

Balancing recall and precision for defaulters

🧰 Tech Stack

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

🚀 How to Run

Open PRCP-1006-HomeLoanDef.ipynb

Install required Python libraries

Run the notebook cells sequentially
