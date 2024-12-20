# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Initialize \( L \) as identity and \( U \) as zero matrices.
2. For each row \( i \), compute \( U[i, j] \) for \( j \geq i \).
3. Compute \( L[j, i] \) for \( j > i \) using the formula for \( L[j, i] \).
4. Return \( L \) and \( U \) such that \( A = L \cdot U \).


## Program:
```
'''Program to find L and U matrix using LU decomposition.
Developed by:Darshini B 
RegisterNumber:24008783
'''

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

'''Program to solve a matrix using LU decomposition.
Developed by:Darshini B
RegisterNumber:24008783
'''

import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)
```
## Output:
![image](https://github.com/user-attachments/assets/1e901939-cb6f-4d5a-a84b-b5b5d5677f1b)
![image](https://github.com/user-attachments/assets/df666c77-c62d-41e2-973e-7d224f22c409)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

