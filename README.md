# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
step1: start
step2: Get the independent variable X and dependent variable Y.
step3: Calculate the mean of the X -values and the mean of the Y -values.
step4: Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
step5: Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
step6: Use the slope m and the y -intercept to form the equation of the line.
step7: Obtain the straight line equation Y=mX+b and plot the scatterplot.
step8: stop
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
