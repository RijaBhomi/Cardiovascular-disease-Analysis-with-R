# Cardiovascular Disease Analysis

## Overview
This project involves data preprocessing, feature engineering, exploratory data analysis (EDA), and visualization for cardiovascular disease prediction using R. The dataset used is `cardio_train.csv`, and the analysis focuses on identifying key health indicators linked to cardiovascular disease.

---

## Prerequisites
Before running the code, ensure you have the following R libraries installed:

```R
install.packages(c("tidyverse", "caret", "glmnet", "randomForest", "xgboost",
                   "cluster", "factoextra", "ggplot2", "kableExtra", "DescTools",
                   "corrplot", "ggpubr", "tibble", "recipes", "rpart.plot", "ROSE", "gridExtra"))
```


#Code Structure

##1. Importing and Preprocessing Data

The dataset is loaded from a CSV file.

Structure, dimensions, and summary statistics of the dataset are displayed.

Missing values and duplicate records are checked.

Data cleaning operations:

Age is converted from days to years.

Gender is recoded (female: 0, male: 1).

Outliers in height, weight, blood pressure, and BMI are filtered.

##2. Feature Engineering

New features added:

BMI (Body Mass Index)

Pulse Pressure (Difference between systolic and diastolic blood pressure)

Age Groups (Categorized age ranges)

BMI Groups (Underweight, Normal, Overweight, Obese)

Risk Score based on key health indicators

##3. Data Export

The cleaned dataset is saved as data_clean.csv for further analysis.

##4. Descriptive Statistics

Interval variables like age, height, weight, and blood pressure are summarized.

Frequency statistics for categorical variables such as gender, cholesterol, glucose, smoking, alcohol intake, and physical activity.

##5. Exploratory Data Analysis (EDA) & Visualizations

Pie Chart: Proportion of patients with and without cardiovascular disease.

Histogram: Age distribution vs. cardiovascular disease.

Boxplots:

Systolic and diastolic blood pressure.

Height and weight.

Bar Charts:

Cholesterol and glucose levels in relation to cardiovascular disease.

BMI group distribution by disease status.

##Key Insights

Older individuals (50+) have a higher prevalence of cardiovascular disease.

High cholesterol and glucose levels are strongly associated with increased disease risk.

Individuals with higher BMI (overweight/obese) tend to have a higher risk of cardiovascular disease.

##Usage

Load the script in RStudio or any R-compatible environment.

Ensure cardio_train.csv is available in the specified directory.

Run the script sequentially to clean data, engineer features, and perform EDA.


##Future Enhancements

Implement predictive modeling (Logistic Regression, Decision Trees, XGBoost).

Perform advanced feature selection.

Improve data visualization with interactive dashboards (e.g., Shiny or Dash for R).





