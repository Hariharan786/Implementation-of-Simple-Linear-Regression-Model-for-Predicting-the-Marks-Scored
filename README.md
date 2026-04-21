# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
**Step 1:** Import the required libraries ,and set up the data (hours studied and marks).
Make sure the input data is in the correct shape for the model.

**Step 2:** Create the linear regression model and train it using the data.
This step helps the model understand how hours and marks are related.

**Step 3:** Get the slope and intercept, then give input to predict marks.
The model uses what it has learned to estimate the result.

**Step 4:** Draw a graph showing the real data and the regression line.
This helps to clearly visualise the relationship between study time and marks.


## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Hariharan Ganesh
RegisterNumber:212225040111

import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression
X=np.array([1,2,3,4,5]).reshape(-1,1)
Y=np.array([25,50,65,70,85])
model=LinearRegression()
model.fit(X,Y)
m=model.coef_[0]
b=model.intercept_
print("Slope(m):",m)
print("intercept(b):",b)
x_input=float(input("Enter hours studied: "))
predicted_marks=model.predict([[x_input]])
print("Predicted Marks:",predicted_marks[0])
Y_pred=model.predict(X)
plt.scatter(X,Y,label="Actual Data")
plt.plot(X,Y_pred,label="RegressionLine")
plt.xlabel("Hours Studied")
plt.ylabel("Marks scored")
plt.title("Simple Linear Regression(Using sklearn)")
plt.legend()
plt.show()
*/
```

## Output:
<img width="759" height="684" alt="Screenshot 2026-04-21 092554" src="https://github.com/user-attachments/assets/aea64476-ebd4-4973-813e-f5e90d73d35c" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
