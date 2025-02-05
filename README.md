# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eq1](https://user-images.githubusercontent.com/118364993/214309218-8e435eab-436b-453c-b317-0e0e92020fae.png)

4.	Compute the y -intercept of the line by using the formula:
![eq2](https://user-images.githubusercontent.com/118364993/214309310-0cae57c8-9a5a-4aca-aa95-ca88bc41003b.png)

5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
Developed by : Tejusve Kabeer.F
Reference.no : 22002543

import numpy as np
import matplotlib.pyplot as plt
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
    num+=(x[i]-xmean)*(y[i]-ymean)
    den+=(x[i]-xmean)**2
m=num/den
b=ymean-m*xmean
print(m,b)
ypred=m*x+b
print(ypred)
plt.scatter(x,y,color='Red')
plt.plot(x,ypred,color='Blue')
plt.show()
```

## Output
![input](https://user-images.githubusercontent.com/118364993/214309958-e66a1705-4a2f-4943-9834-d05fbccf4050.png)


</br>![uni](https://user-images.githubusercontent.com/118364993/214305152-60bc822d-62fd-407a-a264-427fea518e73.png)


</br>
</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
