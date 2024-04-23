ersonal Income Classification

This Python program utilizes pandas, seaborn, scikit-learn libraries to classify individuals into income brackets (<= $50,000 or > $50,000) based on a provided dataset (income.csv). The script performs exploratory data analysis (EDA), data cleaning, feature engineering, and logistic regression modeling.

Key functionalities of the script:

    Data Loading and Preprocessing:
        1.Reads the CSV file using pandas.
        2.Creates a copy of the data for manipulation.
        3.Analyzes data structure and provides summary statistics.
        4.Handles missing values by identifying them and considering " ?" as NaN during data import.
        5.Drops rows with missing values using .dropna(axis=0). Creates copies for further analysis.

    Exploratory Data Analysis (EDA):
        1.Analyzes various features of the dataset using descriptive statistics and visualizations with seaborn.
        2.Identifies potential relationships between features and the target variable (income bracket).
        3.Explores categorical features using value counts and visualizations.

    Data Cleaning:
        1.Addresses potential inconsistencies in the data based on observations from the EDA.

    Feature Engineering:
        1.Encodes categorical variables using one-hot encoding (pd.get_dummies).

    Logistic Regression Modeling:
        1.Splits the data into training and testing sets.
        2.Trains two Logistic Regression models:
        3.One model uses all features.
        4.Another model removes potentially insignificant features (gender, nativecountry, race, JobType) based on domain knowledge or feature importance analysis (not                   included in this script).
        5.Evaluates the performance of both models using accuracy score and misclassified samples.

Outputs:

    1.The program generates various visualizations throughout the script using seaborn to understand the data distribution and feature relationships.
    2.Performance metrics (accuracy score and number of misclassified samples) are printed for both logistic regression models.
    3.A conclusion is not explicitly provided, but you can compare the results of the two models to see if removing features affects the classification accuracy.

Note:

    1.This script assumes the required libraries (pandas, seaborn, scikit-learn) are installed.
    2.The CSV file containing the income data (income.csv) needs to be placed in the same directory as the script.
