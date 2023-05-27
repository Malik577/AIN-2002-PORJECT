# Stroke Prediction Project

## Table of Contents
1. Description
2. Data
3. Files
4. Project Structure
   - Data Import and Merging
   - Data Preprocessing
   - Exploratory Data Analysis & Data Visualization
   - Model Training
   - Final Model Training and Predictions
5. Model Evaluation
6. Usage
7. Authors

## 1. Description
This repository contains a Python-based data science project aimed at predicting stroke events based on various clinical and lifestyle indicators. The project follows a comprehensive data science pipeline, starting from data preprocessing and culminating in machine learning model training, evaluation, and stroke predictions.

## 2. Data

The project uses two datasets from Kaggle:

- *Stroke Prediction Dataset*: A real-world dataset, including various clinical and lifestyle features associated with stroke events. 

- *Synthetic Stroke Prediction Dataset*: This dataset contains synthetic data points generated from a deep learning model trained on the Stroke Prediction Dataset.

Together, these datasets offer a comprehensive set of data points for stroke prediction modeling.

## 3. Files

The repository includes several important files:

- `Stroke-prediction.ipynb`: The primary Python script of the project handling data preprocessing, model training, evaluation, and final stroke predictions.

- `train.csv` and `healthcare-dataset-stroke-data.csv`: CSV files containing the datasets used in the project.

- `test.csv`: CSV file containing the testing dataset used in the project for model evaluation.

- `submission_1.csv`: A CSV file housing the stroke predictions made by the logistic regression model after full dataset training.

- `README.md`: This file provides an overview of the project, the data used, and basic usage instructions.

## 4. Project Structure

The project comprises several crucial steps:

### Data Import and Merging
Two different datasets are imported and merged into a single DataFrame.

### Data Preprocessing
This step involves handling missing values, standardizing numerical features, one-hot encoding categorical features, and removing outliers and logically invalid records.

### Exploratory Data Analysis & Data Visualization
Various bar plots, histograms, correlation heatmaps, and box plots are generated to gain a better understanding of the data and the relationships between different features.

### Model Training
A logistic regression model is trained using Stratified K-Fold cross-validation. The model is evaluated using ROC AUC score and Mean Squared Error (MSE) metrics on both the training and validation sets.

### Final Model Training and Predictions
The logistic regression model is retrained on the full dataset. The model's predictions are saved into 'submission_1.csv'.

## 5. Model Evaluation

The logistic regression model's performance is evaluated based on various metrics. The Stratified K-Fold cross-validation method ensures a fair evaluation by preserving the percentage of samples for each class. 

The metrics used are ROC AUC score and Mean Squared Error (MSE). ROC AUC score measures the area under the receiver operating characteristic (ROC) curve, which provides a comprehensive measure of model performance by considering both sensitivity and specificity. On the other hand, MSE measures the average squared difference between the predicted and actual values.

Confidence intervals for the AUC score are estimated using the bootstrap resampling method, providing a range of possible values for the model's performance.

## 6. Usage

To use this project:

1. Clone this repository.
2. Ensure Python, along with the necessary libraries (pandas, numpy, matplotlib, seaborn, plotly, sklearn), is installed on your machine.
3. Run `stroke_prediction.py

` using a Python interpreter.

## 7. Authors
Qatrlnada Almrzoq 

Malik Alghossein

Abdullah A.A Mahmoud
