Employee Attrition Prediction Using Machine Learning
Project Overview
This project explores the use of supervised machine learning models to predict employee attrition. The primary objective was to build a classification model capable of identifying employees at risk of leaving, with particular emphasis on improving recall for the attrition class.
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


Evaluation Strategy
 Since attrition cases were fewer than non-attrition cases, recall for the attrition class was prioritised over accuracy.
 Additional experiments included class balancing and probability threshold adjustment to improve minority class detection.



Results
Among the evaluated models, Random Forest provided the best balance between recall and overall stability.
Key observations:
Logistic Regression performed reasonably but was limited by its linear decision boundary.


Decision Tree improved recall but showed higher variance.


Random Forest reduced variance and delivered more consistent performance.


Adjusting the classification threshold increased recall but introduced a precision trade-off.


The final model was selected based on alignment with the project objective rather than raw accuracy alone.

Limitations
The dataset is limited in size and represents a single organisational context.


External factors such as economic conditions and personal circumstances were not included.


The analysis identifies associations, not causal relationships.


Model performance may vary over time, requiring monitoring and retraining in real-world deployment.



Tools & Technologies
Python


Pandas


NumPy


Matplotlib / Seaborn


Scikit-learn



Key Takeaway
This project demonstrates a practical application of classification modelling in HR analytics, with emphasis on evaluation strategy, trade-offs, and responsible interpretation of results.
