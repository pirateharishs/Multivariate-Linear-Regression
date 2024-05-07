# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
Import Pandas library.

### Step2:
Import Linear_model from sklearn.

### Step3:
Read the csv file using pandas library.

### Step4:
Enter the parameters of the linear function.

### Step5:
Print the parameters of the linear function.

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
![image](https://github.com/pirateharishs/Multivariate-Linear-Regression/assets/166011385/bec90f42-ac3d-48cf-9ef7-589bcbe29400)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
