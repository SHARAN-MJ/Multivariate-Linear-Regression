# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import oandas as pd
<br>
 
### Step2
read the csv file
<br>

### Step3
<br>
Get the value of X and y variables.


### Step4
<br>
Create the linear regression model and fit.

### Step5
<br>
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

### step6 
 <br>
Print the predicted output.

## Program:
```


import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)



```
## Output:
![output](./Screenshot_20230125_070214.png)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
