Stroke Prediction

By
Qatrlnada Almrzoq 1900678
Malik Alghossein 2101410
Abdullah A.A Mahmoud 2104576

This project focuses on predicting stroke events by analyzing clinical features using real-world and synthetic datasets. The goal is to identify key risk factors for strokes by examining parameters such as gender, age, hypertension, heart disease, and lifestyle choices.

Requirements
To install the required packages, run the following command:

Copy code
pip install -r requirements.txt
Data
Data Source
Dataset: Stroke Prediction Dataset from Kaggle website
Kaggle Dataset 1
Kaggle Dataset 2
The dataset contains the following columns:

id: Patient ID
gender: "Male", "Female" or "Other"
age: Patient's age
hypertension: 0 if the patient does not have hypertension, 1 if the patient has hypertension
heart_disease: 0 if the patient does not have heart disease, 1 if the patient has heart disease
ever_married: "No" or "Yes"
work_type: "children", "Govt_job", "Never_worked", "Private" or "Self-employed"
Residence_type: "Rural" or "Urban"
avg_glucose_level: Average blood sugar level
bmi: Body mass index
smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown"
Data Cleaning
In this project, data cleaning is performed to ensure the dataset is ready for analysis. Missing values in the 'bmi' column are filled with the mean values calculated separately for cases with and without strokes.

Encoding the Variables
To work with categorical variables for further analysis, data encoding is performed. Categorical variables are converted into numerical format using the factorize function, enhancing the dataset's relevance for modeling.

Data Analysis
Correlation analysis is conducted to examine the relationships between variables.

Training
Six different machine learning models from the scikit-learn library are used for training:

GradientBoostingClassifier
SVC
LogisticRegression
DecisionTreeClassifier
Xgboost
RandomForestClassifier
Regressor models are also tested to understand their performance, although they are not suitable for binary classification problems since they are used for continuous variables.

Results
The results of the trained models are not provided in the given information. Please refer to the project's report or documentation for detailed results and performance metrics.


