# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Start the program
2. Enter data Define values of X and Y
3. Find mean Calculate mean of X and mean of Y
4. Calculate slope (m) Use formula to find slope
5. Calculate intercept (b)
6. Use formula to find intercept Find predicted values
Compute  𝑌 = 𝑚𝑋+𝑏
7. Plot graph and display result, then Stop
## Program
```
Program to develop to implement univariate Linear Regression to fit a straight line using least squares.

Developed by :Kabilan S
Register no : 212225230119

import numpy as np
import matplotlib.pyplot as plt
X= np.array([0,1,2,3,4,5,6,7,8,9])
Y= np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(X,Y)
plt.show()
X_Mean=np.mean(X)
Y_Mean=np.mean(Y)
num=0
den=0
for i in range(len(X)):
    num+=(X[i]-X_Mean)*(Y[i]-Y_Mean)
    den+=(X[i]-X_Mean)**2

m=num/den
b=Y_Mean-(m*X_Mean)
print(f"Slope : {m}\nIntercept : {b}")
Y_Pred=(m*X)+b
print(f"Predicted values are : \n{Y_Pred}")
plt.scatter(X,Y,color='Red')
plt.plot(X,Y_Pred,color='Blue')
plt.show()





```
## Output
![exp 9](https://github.com/user-attachments/assets/8a1a1925-4b70-4369-8f68-bdd5b925c0b3)




## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
