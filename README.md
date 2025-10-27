# Predicting Housing Prices Using Regularized Linear Regression Models

##  Overview
This project focuses on predicting **median housing prices (MEDV)** using regression techniques on the **HousingData.csv** dataset. The primary objective is to build a robust model that mitigates **overfitting** using **Ridge**, **Lasso**, and **Elastic Net Regression** methods.

---

##  Dataset Description
The dataset `HousingData.csv` consists of various features that influence housing prices.

| Feature | Description |
|----------|-------------|
| CRIM | Per capita crime rate by town |
| ZN | Proportion of residential land zoned for lots over 25,000 sq.ft. |
| INDUS | Proportion of non-retail business acres per town |
| CHAS | Charles River dummy variable (1 if tract bounds river; 0 otherwise) |
| NOX | Nitric oxides concentration (parts per 10 million) |
| RM | Average number of rooms per dwelling |
| AGE | Proportion of owner-occupied units built prior to 1940 |
| DIS | Weighted distances to five Boston employment centers |
| RAD | Index of accessibility to radial highways |
| TAX | Full-value property-tax rate per \$10,000 |
| PTRATIO | Pupil–teacher ratio by town |
| B | 1000(Bk - 0.63)^2, where Bk is the proportion of Black residents by town |
| LSTAT | % lower status of the population |
| MEDV | Median value of owner-occupied homes (in \$1000s) — **Target Variable** |

---

##  Steps and Methodology

### 1️ Data Preprocessing
- Handled missing values in `CRIM`, `ZN`, `INDUS`, and `CHAS` columns  
- Performed **EDA (Exploratory Data Analysis)** to understand feature correlations  
- Checked for **outliers** and **multicollinearity** using the Variance Inflation Factor (VIF)

### 2️ Model Implementation
Implemented and compared the following regression models:

| Model | Description |
|--------|--------------|
| **Linear Regression** | Baseline model without regularization |
| **Ridge Regression** | L2 regularization to reduce model complexity |
| **Lasso Regression** | L1 regularization for feature selection |
| **Elastic Net Regression** | Combination of L1 and L2 regularization |

### 3️ Model Evaluation
Used standard regression metrics to evaluate model performance:
- Mean Squared Error (MSE)  
- Root Mean Squared Error (RMSE)  
- R² Score  
- Cross-validation for model stability  

---

##  Results
- **Linear Regression** achieved a baseline performance but showed slight overfitting.  
- **Ridge Regression** reduced overfitting by penalizing large coefficients.  
- **Lasso Regression** performed feature selection by driving some coefficients to zero.  
- **Elastic Net** provided a balanced approach between Ridge and Lasso.  

📊 The final model demonstrated improved **generalization** and **stability** across validation sets.
