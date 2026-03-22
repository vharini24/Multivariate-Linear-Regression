# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas and scikit-learn

### Step2
Load dataset using read_csv()

### Step3
Define independent variables 𝑋 and dependent variable 𝑦 

### Step4
Create and train model using LinearRegression().fit(X, y)

### Step5
Predict output using predict() and display results

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:

<img width="767" height="391" alt="image" src="https://github.com/user-attachments/assets/cea37b57-caf7-44f1-879e-3833d241e5ca" />

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
