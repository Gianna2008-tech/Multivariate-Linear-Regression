# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Organize features into a matrix and add a column of ones for bias.

### Step2
Compute the coefficients using the Normal Equation.
### Step3
redict outputs for new inputs by multiplying with the coefficients.

### Step4
Return the coefficients and predicted values.


## Program:
```

#Program to implement multivariate linear regression and predict the output.
#Developed by: GIANNA J
#Reg no : 25011912
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)





```
## Output:
<img width="1020" height="249" alt="Screenshot 2025-12-18 185635" src="https://github.com/user-attachments/assets/95f95f75-df0e-4609-9be7-a678e5d70993" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
