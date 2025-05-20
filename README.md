# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import Pandas library.

### Step2
<br>
Import Linear_model from sklearn.

### Step3
<br>
Read the csv file using pandas library.

### Step4
<br>
Enter the parameters of the linear function.


### Step5
<br>

Print the parameters of the linear function.

## Program:
```python
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
### Insert your output
![Screenshot 2025-05-17 102914](https://github.com/user-attachments/assets/e5adb439-25f8-4f56-98f7-b705ccb72de8)
<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
