# HealAThon-Team-K
prediction of whether a patient has prostate cancer or not

## Introduction: 

This project involves the steps taken to predict the log of PSA (lpsa) from a set of measurements including log cancer volume (lcavol), log prostate weight (lweight), age, log of benign prostatic hyperplasia amount (lbph), seminal vesicle invasion (svi), log of capsular penetration (lcp), Gleason score (gleason), and percent of Gleason scores 4 or 5 (pgg45). 

## Data Preprocessing: 

I started by loading the dataset into a pandas dataframe and checking for missing values. I then defined the numerical and categorical columns and checked for outliers using the IQR method. I also checked for skewness in numerical columns and applied log transformation to highly skewed numerical columns. Finally, I scaled numerical variables using the StandardScaler. 

 
## Exploratory Data Analysis: 

I visualized the distributions of numerical columns to gain insights and identify any patterns. I also looked at the correlation between features and the target variable to determine the most important features in predicting lpsa. 

## Model Selection and Evaluation: 

I trained and evaluated multiple regression models including Linear Regression, Lasso, Ridge, Decision Tree Regressor, and Random Forest Regressor. I used the mean squared error (MSE) and R-squared metrics to evaluate the performance of each model. Based on the evaluation, Ridge Regression was selected as the best model with a RMSE of 0.5547836725838953 and R-squared of 0.7463937818109245. 

## Conclusion: 

In conclusion, I was able to successfully predict the log of PSA (lpsa) using Ridge Regression. The most important features in predicting lpsa were log cancer volume, log prostate weight, seminal vesicle invasion, log of capsular penetration, and patient age. This information can be used to improve the diagnosis and treatment of prostate cancer. 


## Usage
Git clone and run the Prostrate_Cancer.ipynb file using Python Jupyter Notebook
