Employee Attrition Prediction Using Machine Learning
Project Overview

This project explores the use of supervised machine learning models to predict employee attrition. The primary objective was to build a classification model capable of identifying employees at risk of leaving, with emphasis on improving recall for the attrition class.

Rather than focusing solely on overall accuracy, this analysis prioritises correctly identifying employees likely to leave, reflecting the higher organisational cost of false negatives in attrition prediction.

Dataset

The dataset contains 1,470 employee records with demographic, compensation, and work-related attributes.

Key features include:

Monthly Income

Age

Overtime status

Job-related and tenure-related variables

The target variable indicates whether an employee left the organisation.

Methodology

The project followed a structured workflow:

Exploratory Data Analysis (EDA)

Examined relationships between employee characteristics and attrition. Monthly income, age, and overtime showed noticeable associations with attrition rates.

Data Preparation

Train–test split

Feature encoding

Scaling where appropriate

Careful handling to avoid data leakage

Model Development

The following models were evaluated:

Logistic Regression (baseline)

Decision Tree

Random Forest

Evaluation focused on recall due to class imbalance, and threshold adjustment was applied to improve minority class detection.

Results

Random Forest delivered the most balanced and stable performance, particularly in detecting attrition cases. The final model was selected based on alignment with the project objective rather than overall accuracy alone.

Limitations

Limited dataset size

No external factors included

Associations identified, not causal relationships

Model performance may vary over time

Tools & Technologies

Python

Pandas

NumPy

Matplotlib / Seaborn

Scikit-learn



Key Takeaway
This project demonstrates a practical application of classification modelling in HR analytics, with emphasis on evaluation strategy, trade-offs, and responsible interpretation of results.

