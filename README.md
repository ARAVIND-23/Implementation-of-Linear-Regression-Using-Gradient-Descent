# Implementation-of-Linear-Regression-Using-Gradient-Descent

## AIM:
To write a program to predict the profit of a city using the linear regression model with gradient descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. To train, initialize theta and iteratively update it using gradient descent.
2. For preprocessing, read and scale data.
3. For modeling, train the linear regression model.
4. To predict data values, scale a new data and predict.
5. Print the prediction.
 

## Program & Output:
```
/*
Program to implement the linear regression using gradient descent.
Developed by: ARAVIND G
RegisterNumber: 212223240011 
*/
```
```
import pandas as pd import numpy as np from sklearn.metrics import mean_absolute_error,mean_squared_error import matplotlib.pyplot as plt df=pd.read_csv("student_scores.csv") print(df.head()) print(df.tail())
```
![Screenshot 2024-11-11 224552](https://github.com/user-attachments/assets/f579f6e8-7cd5-4593-a6ba-63e4274a8275)
```
x=df.iloc[:,:-1].values print(x) y=df.iloc[:,-1].values print(y)
```
![Screenshot 2024-11-11 224702](https://github.com/user-attachments/assets/f74a1b41-da1d-4c7e-be5c-efa7ca496d07)
```
x.shape y.shapem=0 c=0 L=0.001 # learning rate epochs=5000 # No.of iterations to be performed n=float(len(x)) error=[]
```
## Performing Gradient Descent:
```
for i in range(epochs): y_pred = mx + c D_m = (-2/n)sum(x(y-y_pred)) D_c = (-2/n)sum(y-y_pred) m = m-LD_m c = c-LD_c error.append(sum(y-y_pred)**2) print(m,c) type(error) print(len(error)) plt.plot(range(0,epochs),error)
```
![Screenshot 2024-11-11 224936](https://github.com/user-attachments/assets/ae93276e-76fe-4801-8d5d-fa8d2992176f)
![Screenshot 2024-11-11 225015](https://github.com/user-attachments/assets/89de5b38-7502-4db9-8f85-26a2395c9f7e)


## Result:
Thus the program to implement the linear regression using gradient descent is written and verified using python programming.
