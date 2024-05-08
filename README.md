# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Step1:
import pandas as pd.

## Step2:
Read the csv file.

## Step3:
Get the value of X and y variables.

## Step4:
Create the linear regression model and fit.

## Step5:
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm
cube.

## Program:
```
#Program to implement multivariate linear regression and predict the output.
#Developed by: HARISH S
#RegisterNumber: 212223230071
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("GT.csv")
X=df[['Weight','Volume']]
Y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)


```
## Output:

![image](https://github.com/pirateharishs/Multivariate-Linear-Regression/assets/166011385/621ce114-a71c-4646-8995-6b2f8c433dd8)
![image](https://github.com/pirateharishs/Multivariate-Linear-Regression/assets/166011385/04e4083d-f14b-4c16-b351-bc90e44a5d07)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
