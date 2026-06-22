# House Price Prediction Model

## Project Overview

This project focuses on predicting house prices using Machine Learning Regression techniques. The Housing Dataset was analyzed, preprocessed, and used to train predictive models. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, model training, evaluation, and comparison of different regression algorithms.

---

## Objective

The objective of this project is to build a machine learning model capable of predicting house prices based on various housing features such as area, number of bedrooms, bathrooms, stories, parking availability, furnishing status, and other amenities.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Statsmodels

---

## Dataset

Dataset Used: Housing.csv

The dataset contains information about houses and their corresponding prices.

### Features

- Price
- Area
- Bedrooms
- Bathrooms
- Stories
- Main Road Access
- Guest Room
- Basement
- Hot Water Heating
- Air Conditioning
- Parking
- Preferred Area
- Furnishing Status

---

## Project Workflow

### 1. Data Loading

- Loaded Housing.csv dataset using Pandas.
- Examined dataset structure and information.

### 2. Data Preprocessing

- Checked missing values.
- Checked duplicate records.
- Verified data types.
- Handled categorical features using One-Hot Encoding.

### 3. Exploratory Data Analysis (EDA)

- Distribution plots (Histograms)
<img width="986" height="739" alt="image" src="https://github.com/user-attachments/assets/9154b134-a879-4999-96ac-c1b1f1af5587" />

- Boxplots for outlier detection
<img width="826" height="588" alt="image" src="https://github.com/user-attachments/assets/3bd8c6ef-3d94-4d6f-ae2e-771d2feb35cd" />

- Correlation Heatmap
<img width="757" height="528" alt="image" src="https://github.com/user-attachments/assets/65e91b75-1dec-45e1-bec7-1d9bb7e3db1c" />

- Area vs Price Scatter Plot
<img width="691" height="470" alt="image" src="https://github.com/user-attachments/assets/3ad6b865-4bb1-4289-bb9a-daf07ea69407" />

- Bedrooms vs Price Analysis
<img width="691" height="470" alt="image" src="https://github.com/user-attachments/assets/8066ebeb-325f-402f-b6be-50aaa982cb42" />


### 4. Feature Engineering

Categorical variables were transformed using One-Hot Encoding:

- mainroad
- guestroom
- basement
- hotwaterheating
- airconditioning
- prefarea
- furnishingstatus

### 5. Multi-Collinearity Analysis

Variance Inflation Factor (VIF) was used to check multi-collinearity among independent variables.

### 6. Model Building

#### Linear Regression

A Linear Regression model was trained using the processed dataset.

#### Ridge Regression

A Ridge Regression model was also trained and evaluated for comparison.

### 7. Model Evaluation

The following metrics were used:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## Results

### Linear Regression

- MAE ≈ 970,043
- RMSE ≈ 1,324,507
- R² Score ≈ 0.653

### Ridge Regression

- MAE ≈ 970,246
- RMSE ≈ 1,325,320
- R² Score ≈ 0.652

### Model Comparison

| Model | R² Score |
|---------|---------|
| Linear Regression | 0.653 |
| Ridge Regression | 0.652 |

Linear Regression achieved slightly better performance and was selected as the final model.

---

## Conclusion

The House Price Prediction Model was successfully developed using Machine Learning Regression techniques. Data preprocessing, One-Hot Encoding, exploratory data analysis, and multi-collinearity checks were performed. The Linear Regression model achieved the best performance with an R² score of approximately 0.653 and can be used for predicting house prices based on housing characteristics.
