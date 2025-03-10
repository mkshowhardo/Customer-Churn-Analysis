# Customer Churn Analysis

This project aims to analyze customer churn for a telecommunications company using machine learning and data visualization techniques. The dataset contains information about customer demographics, account information, and whether the customer has churned or not. The goal of the analysis is to predict customer churn, identify patterns, and provide actionable insights for reducing churn.

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis](#exploratory-data-analysis)
5. [Modeling](#modeling)
6. [Visualizations](#visualizations)
7. [Key Insights](#key-insights)
8. [Installation](#installation)
9. [Usage](#usage)
10. [Contributing](#contributing)

## Introduction
Customer churn refers to the loss of customers over time, which is a major concern for any business. This analysis helps to understand the factors contributing to churn and provides insights into customer behavior. By predicting churn, businesses can take proactive measures to retain valuable customers.

## Dataset
The dataset used in this analysis is the **Customer Churn** dataset from a telecommunications company. It includes the following columns:

- **CustomerID**: Unique identifier for each customer
- **Gender**: Gender of the customer
- **SeniorCitizen**: Whether the customer is a senior citizen (1 or 0)
- **Partner**: Whether the customer has a partner (Yes or No)
- **Dependents**: Whether the customer has dependents (Yes or No)
- **Tenure**: The number of months the customer has been with the company
- **PhoneService**: Whether the customer has phone service (Yes or No)
- **MultipleLines**: Whether the customer has multiple lines (Yes or No)
- **InternetService**: Type of internet service (DSL, Fiber optic, or No)
- **OnlineSecurity**: Whether the customer has online security (Yes or No)
- **OnlineBackup**: Whether the customer has online backup (Yes or No)
- **DeviceProtection**: Whether the customer has device protection (Yes or No)
- **TechSupport**: Whether the customer has tech support (Yes or No)
- **StreamingTV**: Whether the customer has streaming TV (Yes or No)
- **StreamingMovies**: Whether the customer has streaming movies (Yes or No)
- **PaperlessBilling**: Whether the customer has paperless billing (Yes or No)
- **PaymentMethod**: Payment method used by the customer
- **MonthlyCharges**: The amount the customer is charged monthly
- **TotalCharges**: The total amount the customer has been charged
- **Churn**: Whether the customer has churned (Yes or No)

## Data Preprocessing
The data was preprocessed to handle missing values, convert categorical columns into numerical values, and normalize numerical features. The preprocessing steps include:

1. **Handling Missing Values**: Missing values in critical columns like `Churn` and `Contract` were handled.
2. **Converting Categorical to Numeric**: Categorical columns such as `Churn`, `Contract`, and others were converted into numeric values for easier analysis.
3. **Scaling**: Numerical features were scaled to ensure consistent data ranges.

## Exploratory Data Analysis
Various exploratory data analysis (EDA) techniques were used to uncover insights, including:

- Distribution of churned vs. non-churned customers
- Correlation between features such as `MonthlyCharges` and `Churn`
- Visualizations to understand trends and patterns in customer behavior

## Modeling
A machine learning model was created to predict customer churn. The following steps were followed:

1. **Data Splitting**: The dataset was split into training and testing sets.
2. **Modeling**: A logistic regression model was trained to predict churn.
3. **Evaluation**: The model was evaluated using metrics like accuracy, precision, recall, and F1-score.

## Visualizations
Several visualizations were created to better understand the data and the results of the analysis:

- **Churn Rate**: Pie charts to show the proportion of churned vs. non-churned customers.
- **Churn by Contract Type**: Bar charts to compare churn rates by contract type (Month-to-month, One year, etc.).
- **Churn by Monthly Charges**: Box plots and scatter plots to explore how monthly charges correlate with churn.

## Key Insights
Some key insights gained from this analysis include:

- Customers with month-to-month contracts have a higher churn rate than those with longer-term contracts.
- Customers with higher monthly charges tend to have a higher churn rate.
- Offering more personalized plans and incentives can help reduce churn, especially for month-to-month customers.

## Installation

To use or contribute to this project, clone the repository and install the required libraries:

```bash
git clone https://github.com/your-username/customer-churn-analysis.git
cd customer-churn-analysis
pip install -r requirements.txt
python churn_analysis.py
