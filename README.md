# Used Car Price Prediction with Machine Learning

This end-to-end machine learning project aims to **predict the selling price of used cars** using multiple regression models. It covers **data preprocessing, exploratory data analysis (EDA), feature engineering, model building, evaluation**, and performance comparison — everything needed to turn raw data into actionable predictions.

---

## Project Objective
To build a regression model that accurately estimates the **resale price of a used car**, helping:
- Sellers list competitive prices
- Buyers determine fair market value

---

## Tools & Technologies
- **Language**: Python
- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost
- **IDE**: Jupyter Notebook
- **Version Control**: Git & GitHub

---

## Dataset Overview
- **Records**: 19,980 used cars
- **Target**: `selling_price`
- **Features**:
  - `full_name` (brand & model)
  - `year`, `km_driven`, `fuel_type`, `transmission_type`
  - `mileage`, `engine`, `max_power`, `seats`, `seller_type`

---

## Key Steps Performed

### 1. Data Cleaning
- Removed 0 mileage rows
- Capped extreme outliers in `selling_price`
- Converted `year` to `age`

### 2. Feature Engineering
- Binned `seats` (2–4, 5, >5)
- Extracted `make` and `model` from `full_name`
- One-hot encoded categorical variables
- Scaled numerical features using `MinMaxScaler`

### 3. Exploratory Data Analysis
- Visualized distributions
- Checked for multicollinearity
- Identified key relationships with `selling_price`

### 4. Model Building & Evaluation
Models used:
- Linear Regression
- Ridge & Lasso Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Stochastic Gradient Boosting
- XGBoost (Best performer)

### 5. Metrics
- R² Score
- Mean Squared Error (MSE)
- K-Fold Cross Validation

---

## Best Model: XGBoost
| Metric        | Score      |
|---------------|------------|
| Train R²      | 0.9646     |
| Test R²       | 0.9837     |
| Generalization| Excellent |

