# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy module to use the built-in functions for calculation

2. Prepare the lists from each linear equations and assign in np.array()

3. Using the np.zeros(), we can find the solutions.

4. End the program



## Program:
```
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: SAKTHIVEL R
RegisterNumber: 22009121
import numpy as np
n=int(input())
arr=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        arr[i][j]=int(input())
for i in range(n):
    for j in range(i+1,n):
        ratio=arr[j][i]/arr[i][i]
        for k in range(n+1):
            arr[j][k]=arr[j][k]-ratio*arr[i][k]
x[n-1]=arr[n-1][n]/arr[n-1][n-1]

```

## Output:

![Screenshot from 2023-01-11 23-38-16](https://user-images.githubusercontent.com/120550359/211884463-ca524d62-dba3-4c76-b861-9a73864eff51.png)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

