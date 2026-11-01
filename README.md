Project Overview
This project uses the Logistic Regression algorithm to predict whether a person's salary exceeds a specific threshold based on demographic and professional information. The model is trained using historical data and can be used for binary classification tasks.

Objective
The main objective of this project is to build a machine learning model that can classify salary categories based on input features such as age, work experience, and estimated salary.

Dataset Information
The dataset contains the following features:
Feature	DescriptionAge	Age of the individual
EstimatedSalary	Estimated annual salary
YearsExperience	Years of professional experience (if available)
Purchased/Salary Category	Target variable indicating the salary class
Target Variable
0 = Salary below threshold
1 = Salary above threshold
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Project Workflow
1. Data Collection
Load the dataset using Pandas.
Understand the structure and data types.
2. Data Preprocessing
Check for missing values.
Remove duplicates.
Handle outliers if required.
Feature selection.
Exploratory Data Analysis (EDA)
Statistical summary.
Distribution plots.
Correlation analysis.
Boxplots and histograms.
4. Data Splitting
Split the dataset into:
Training Set (80%)
Testing Set (20%)
5. Feature Scaling
Apply StandardScaler to normalize numerical features.
from sklearn.preprocessing import StandardScaler
scaler = StandardScaler()
X_train = scaler.fit_transform(X_train)
X_test = scaler.transform(X_test)
6. Model Training
Train the Logistic Regression model.
from sklearn.linear_model import LogisticRegression
model = LogisticRegression()
model.fit(X_train, y_train)
7. Model Evaluation
Evaluate the model using:
Accuracy Score
Confusion Matrix
Classification Report
from sklearn.metrics import accuracy_score
accuracy = accuracy_score(y_test, y_pred)

Results
The Logistic Regression model successfully predicts salary categories based on the provided input features. Model performance is evaluated using standard classification metrics.

Conclusion
This project demonstrates how Logistic Regression can be used to solve a binary classification problem. The model learns patterns from the dataset and predicts salary categories efficiently, making it a good introductory machine learning project.

Author: Krishna Priya G
Algorithm Used: Logistic Regression
Programming Language: Python
Library: Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
