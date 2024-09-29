# Credit Risk Analysis Mini Project



## Overview
This project aims to analyze credit risk using a dataset containing various customer attributes. The goal is to predict whether a person has good or bad credit risk based on their characteristics, employing logistic regression for classification.

## Results and Conclusion
This model serves as a valuable tool for banks, enabling them to efficiently assess potential credit risks based on readily available customer information. By identifying high-risk customers early in the process, banks can save time and resources before conducting more detailed evaluations. The model achieved an accuracy of approximately 78% on the test set, with a confusion matrix revealing the performance across different classes of credit risk.
This project provides a foundational approach to credit risk analysis using logistic regression. Future improvements could include experimenting with more advanced models and feature engineering techniques.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Data Description](#data-description)
- [Data Visualization](#data-visualization)
- [Data Management](#data-management)
- [Model Training](#model-training)

## Installation
To run this project, you will need Python and the following libraries:
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- scikit-learn

## Usage
1. Clone this repository to your local machine.
2. Update the file paths in the code to point to your datasets (`credit_s.csv` and `credit_g.csv`).
3. Run the Python script to execute the analysis.

## Data Description
Two datasets are utilized in this project:

1. **credit_s.csv**: Contains customer attributes but lacks a target variable for credit risk.
   - Features include: 
     - `Age` (numeric)
     - `Sex` (text): male, female
     - `Job` (numeric): 0 - unskilled and non-resident, 1 - unskilled and resident, 2 - skilled, 3 - highly skilled
     - `Housing` (text): own, rent, or free
     - `Saving` (text): little, moderate, quite rich, rich
     - `Checking` (text): little, moderate, rich
     - `Credit_amount` (numeric, in DM)
     - `Duration` (numeric, in months)
     - `Purpose` (text): various categories

2. **credit_g.csv**: Contains customer attributes along with the target variable for credit risk.
   - Key columns after renaming:
     - `status`: Credit risk status (1 for good, 2 for bad)
     - `Duration`: Duration of the credit
     - `Credit_amount`: Amount of credit
     - `Credit_risk`: Target variable

## Data Visualization
The following visualizations are created to understand the dataset better:
- **Pie chart** for `Credit_risk`
- **Histogram** for `Age`
- **Boxplot** comparing `Age` distributions by `Credit_risk`
- **Bar plot** comparing `Credit_risk` across different `Sex` groups
- **Scatterplot** showing the relationship between `Age` and `Credit_amount` colored by `Credit_risk`

## Data Management
- Summary statistics for key features are calculated.
- Missing values are handled by encoding them as a new category: "Unknown."
- Categorical variables are converted to dummy variables.

## Model Training
A logistic regression model is trained using the processed dataset:
- The data is split into training and testing sets, reserving 20% for testing.
- Cross-validation is used to find the optimal model parameters.
