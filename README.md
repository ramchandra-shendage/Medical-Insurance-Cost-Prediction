# Medical-Insurance-Cost-Prediction
ACME Insurance Inc. offers affordable health insurance to thousands of customer all over the United States . The task to  create an automated system to estimate the annual medical expenditure for new customers, using information such as their age, sex, BMI, children, smoking habits and region of residence. 

I used three regression models in this project:

- Linear Regression
- Ridge Regression
- Lasso Regression

## What I did

The project mainly covers the following steps:

- Loaded and explored the insurance dataset
- Performed basic data analysis and visualization
- Checked distributions, correlations, and outliers
- Handled extreme BMI values using percentile-based trimming
- Split the data into training and testing sets
- Used One-Hot Encoding for categorical variables
- Standardized numerical variables
- Built Linear, Ridge, and Lasso Regression models
- Used 5-fold cross-validation for model comparison
- Used GridSearchCV to find suitable alpha values for Ridge and Lasso
- Compared the models using R², RMSE, and MAE
- Performed residual analysis for Linear Regression

## Models Used

**Linear Regression**  
Used as the basic regression model and as a reference for comparing the regularized models.

**Ridge Regression**  
Used L2 regularization to reduce the effect of large coefficients.

**Lasso Regression**  
Used L1 regularization, which can also shrink some coefficients towards zero.

## Evaluation Metrics

The models were compared using:

- **R² Score**
- **RMSE (Root Mean Squared Error)**
- **MAE (Mean Absolute Error)**

I also used **5-fold cross-validation** to get a more reliable comparison between the models.

## Libraries Used

```text
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Statsmodels
```

## Dataset

The dataset used in this project is `expenses.csv` obtained from kaggle .

The target variable is **`charges`**, which represents the medical insurance charges.

## Conclusion

The main purpose of this project was to understand how Linear Regression and regularization methods like Ridge and Lasso can be used for predicting insurance charges, and to compare their performance using different evaluation methods.
