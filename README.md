# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
```
STEP1: start

STEP2: Get the independent variable X and dependent variable Y.

STEP3: Calculate the mean of the X -values and the mean of the Y -values.

STEP4: Find the slope m of the line of best fit using the formula. 

STEP5: Compute the y -intercept of the line by using the formula:

STEP6: Use the slope m and the y -intercept to form the equation of the line.

STEP7: Obtain the straight line equation Y=mX+b and plot the scatterplot.

STEP8: stop
```
## Program:
```
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
denom=0
for i in range(len(x)):
  num+=(x[i]-x_mean)*(y[i]-y_mean)
  denom+=(x[i]-x_mean)**2
m=num/denom
b=y_mean-m*x_mean
print(m,b)
y_pred=m*x+b
print(y_pred)
plt.scatter(x,y)
plt.plot(x,y_pred,color='red')
plt.show()
```



## Output:
![Screenshot 2024-02-19 204933](https://github.com/SanjayK2006/Find-the-best-fit-line-using-Least-Squares-Method/assets/144979178/318a8b0a-ca8a-4c9d-911b-1fa2b7d54b1e)





## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
