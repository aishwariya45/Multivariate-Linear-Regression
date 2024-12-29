# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Step1
Load the data (e.g., from "car.csv").

## Step2
Separate the features (Volume, Weight) and the target (CO2).

## Step3
Train a linear regression model on the data.

## Step4
Print the coefficients and intercept from the trained model.

## Step5
Make a prediction for new data (e.g., Volume = 100, Weight = 929).

## Step6
Print the predicted CO2 emissions.

## Program:
```

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:\\Users\\admin\\Downloads\\car.csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("Coefficient",regression.coef_)
print("Intercept",regression.intercept_)
print("CO2 required is",regression.predict([[100,929]]))




```
## Output:

### Insert your output
![image](https://github.com/user-attachments/assets/31e03533-8930-4bd8-bfa0-18f40e8ffc6d)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
