# Predicting-Kidney-Disease
Classification and Logistic Regression model in predicting Kidney Disease in Patients

Data science process as follows:
1. Define the problem.

**Real-world problem**: Develop a medical diagnosis test that is better than our current diagnosis system for CKD.

**Data science problem**: Develop a medical diagnosis test that reduces both the number of false positives and the number of false negatives.


2. Obtain the data.

Interested in the pattern between BP, Hypertension, Diabetis and Coronary Artery Disease in contributing to having CKD or not.

3. Explore the data.

If I drop every rows that have null values, the number of rows will be reduced from 400 to 160. The downsides are:
- Loss of valuable informations
- Data sample too small, might not enough for good distribution.


4. Model the data.

Impute missing values with mode Imputation & Predictive Imputation

5. Evaluate the model.

class_ckd
1.0    0.616667
0.0    0.383333

ROC AUC = 0.98

6. Answer the problem.

Answer:
I want to increase:
    1. Accuracy, as I am interested in people who truly has CKD and without CKD.
    2. Sensitivity, as it's more important to know all the patients who has CKD (TP), especially those wrongly diagnosed as not having CKD but actually has.
    3. Precision, because we want to increase the real patients who truly has CKD (TP), and minimize the ones that have False Positive.
