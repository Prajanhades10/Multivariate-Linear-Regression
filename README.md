# Implementation of Multivariate Linear Regression


## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

### Step 1 : Import Pandas library.

### Step 2 : Import Linear_model from sklearn.

### Step 3 : Read the csv file using pandas library.

### Step 4 : Enter the parameters of the linear function.

### Step 5 : Print the parameters of the linear function.



## Program:

```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
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
<img width="1415" height="217" alt="Screenshot 2025-10-17 115020" src="https://github.com/user-attachments/assets/d71597b2-2d99-4854-9f2a-46cf78d69b29" />




## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
