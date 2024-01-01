# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. First,we want to import numpy,then import sys,assume a variable

2. For gaussian method,we want to make 2nd and 3rd column zero
3. For that we want to make a range according to your output
4. Then print the program with the correct form then the output will display


## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by:R.Subhashri 
RegisterNumber:23012776
import sys
import numpy as np
n=int(input())
matrix=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        matrix[i][j]=int(input())
for i in range(n):
    if matrix[i][j]==0.0:
        sys.exit("Divide by zero error")
    for j in range(i+1,n):
        ratio=matrix[j][i]/matrix[i][i]
        for k in range(n+1):
            matrix[j][k]=matrix[j][k]-ratio*matrix[i][k]
x[n-1]=matrix[n-1][n]/matrix[n-1][n-1]
for i in range(n-2,-1,-1):
    x[i]=matrix[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-matrix[i][j]*x[j]
    x[i]=x[i]/matrix[i][i]
for i in range(n):
    print("X%d = %0.2f" %(i,x[i]),end=" ")
*/
```


## Output:



![Screenshot 2024-01-01 094230](https://github.com/SubhashriRavichandran10/Gaussian/assets/145743413/8109aefc-61ee-4cd7-8286-fe56259ea147)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

