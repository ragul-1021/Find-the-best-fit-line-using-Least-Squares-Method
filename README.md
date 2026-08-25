# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
from sklearn.linear_model import LinearRegression
import matplotlib.pyplot as plt

x=[[1],[2],[3],[4],[5]]
y=[2,4,5,4,5]
model= LinearRegression()
model.fit(x,y)
predict=model.predict(x)
print(predict)
print(x , y)
print(model.coef_[0])
print(model.intercept_)

plt.scatter(x,y,color='blue',label='actual data')
plt.plot(x,predict,color='green',label='mx+c')
plt.xlabel("hour studied")
plt.ylabel("mark scored")
plt.title("linear Regression")
plt.legend()
plt.show()
```
## Output:

<img width="771" height="662" alt="image" src="https://github.com/user-attachments/assets/cca4da92-c39f-4e8e-8e94-98def4209d21" />

## Result:

Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
