# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Form the augmented matrix of the system of equations.
2.Apply forward elimination to convert the matrix into upper triangular form.
3.Perform back substitution to solve variables starting from the last equation.
4.Output the solution and end the program.


## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: Krithik kiran S
RegisterNumber: 212225230145
import sys
n=int(input())
a=[]
for i in range(n):
    row=[]
    for j in range(n+1):
        row.append(float(input()))
    a.append(row)
x=[0]*n
for i in range(n):
    if a[i][i]==0:
        sys.exit("Error")
        
    for j in range(i+1,n):
       r=a[j][i]/a[i][i]
       for k in range(n+1):
            a[j][k]= a[j][k] - r*a[i][k]

for i in range(n-1,-1,-1):
    x[i]=a[i][n]
    for j in range(i+1,n):
        x[i]-=a[i][j]*x[j]
    x[i]/=a[i][i]
for i in range(n):
    print(f"X{i} = {x[i]:.2f}",end=" ")

*/
```

## Output:

<img width="1920" height="1080" alt="Screenshot (107)" src="https://github.com/user-attachments/assets/bea8b274-54a2-46a4-9384-d6fca6b4104f" />



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

