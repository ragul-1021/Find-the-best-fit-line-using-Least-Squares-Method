Implementation of Univariate Linear Regression
AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

Equipments Required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Jupyter notebook
Algorithm
Get the independent variable X and dependent variable Y.
Calculate the mean of the X -values and the mean of the Y -values.
Find the slope m of the line of best fit using the formula.
image

4. Compute the y -intercept of the line by using the formula:
image

5. Use the slope m and the y -intercept to form the equation of the line. 6. Obtain the straight line equation Y=mX+b and plot the scatterplot.
Program:
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

Output:
image
Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
