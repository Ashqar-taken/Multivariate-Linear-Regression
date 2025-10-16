# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
**Step1**
<br>
Import  the Pandas library and import LinearRegression model using sklearn.linear_model

**Step2**
<br>
Using the method "read_csv" import the dataset csv file.

**Step3**
<br>
Define the Multivariate Independent variable X and Dependent variable Y

**Step4**
<br>
Fit the dataset to the linear regression model

**Step5**
<br>
Now, the model is trainded, Predict the value for a new independent value and print the Co-efficent and intercept of the model and also display the predicted value

## Program:
<br>

```
# Developed By: Ashqar Ahamed S.T
# Register No: 212224240018

import pandas as pd

df = pd.read_csv(r"C:\College\SEM 3\Maths for AI\Lab Experimnets\Exp10\car (1).csv")
#print(df)
X = df[['Weight','Volume']]
Y = df['CO2']

from sklearn.linear_model import LinearRegression

transform = LinearRegression()
transform.fit(X,Y)

print("Co-efficient: ",transform.coef_)
print("Intercept: ",transform.intercept_)

predCO2 = transform.predict([[3300,1300]])
print("Predicted Values: ",predCO2)

```

## Output:
<br>
<img width="899" height="923" alt="image" src="https://github.com/user-attachments/assets/cbf3b144-9a5d-4b5e-a386-1918509a7ce6" />



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
