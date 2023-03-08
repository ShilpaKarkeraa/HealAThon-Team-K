# HealAThon-Team-K

![prostate_cancer](https://user-images.githubusercontent.com/111196709/223775929-1f16162e-3d85-400b-af25-c087984b4fac.jpeg)

## Introduction: 

Prostate cancer is a prevalent type of cancer that affects men, and early detection is essential for effective treatment.
One way to predict prostate cancer is through the log of prostate-specific antigen (PSA) levels, as elevated PSA levels can indicate the presence of cancer. 

This project involves the steps taken to predict the log of PSA (lpsa) from a set of measurements including log cancer volume (lcavol), log prostate weight (lweight), age, log of benign prostatic hyperplasia amount (lbph), seminal vesicle invasion (svi), log of capsular penetration (lcp), Gleason score (gleason), and percent of Gleason scores 4 or 5 (pgg45). 

## Data Preprocessing: 

I started by loading the dataset into a pandas dataframe and checking for missing values. I then defined the numerical and categorical columns and checked for outliers using the IQR method. I also checked for skewness in numerical columns and applied log transformation to highly skewed numerical columns. Finally, I scaled numerical variables using the StandardScaler. 

<img width="640" alt="Screenshot 2023-03-08 at 8 48 04 PM" src="https://user-images.githubusercontent.com/111196709/223776591-42e83869-e2c3-42c5-8a83-4f741607df3f.png">

 
## Exploratory Data Analysis: 

I visualized the distributions of numerical columns to gain insights and identify any patterns. I also looked at the correlation between features and the target variable to determine the most important features in predicting lpsa. 

## Model Selection and Evaluation: 

I trained and evaluated multiple regression models including Linear Regression, Lasso, Ridge, Decision Tree Regressor, and Random Forest Regressor. I used the mean squared error (MSE) and R-squared metrics to evaluate the performance of each model. Based on the evaluation, Ridge Regression was selected as the best model with a RMSE of 0.5547836725838953 and R-squared of 0.7463937818109245.

<img width="640" alt="Screenshot 2023-03-08 at 8 52 32 PM" src="https://user-images.githubusercontent.com/111196709/223777463-0c772d54-092f-473a-962b-da46a98c88af.png">

## Conclusion: 

In conclusion, I was able to successfully predict the log of PSA (lpsa) using Ridge Regression. The most important features in predicting lpsa were log cancer volume, log prostate weight, seminal vesicle invasion, log of capsular penetration, and patient age. This information can be used to improve the diagnosis and treatment of prostate cancer. 
<img width="700" alt="Screenshot 2023-03-08 at 8 54 35 PM" src="https://user-images.githubusercontent.com/111196709/223777885-7be1b185-4582-4db3-9d8a-723c1e0cb76b.png">


## Usage
Git clone and run the Prostrate_Cancer.ipynb file using Python Jupyter Notebook
