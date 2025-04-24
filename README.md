# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

# Step 1:
Import required libraries numpy and scipy.linalg.

# Step 2:
Input the matrix/matrices using eval(input()).

# Step 3:
Perform LU decomposition using lu() or solve equations using lu_factor() and lu_solve().

# Step 4:
Print the results L and U matrices or solution X matrix

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: RISHIVARMAN R
RegisterNumber: 212224100050
'''
import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by:Rishivarman.R 
RegisterNumber: 212224100050
'''
import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu, piv), b)
print(X)
```

## Output:
# (i) L and U matrix
![Screenshot 2025-04-24 220732](https://github.com/user-attachments/assets/9ed7f02d-1caa-4476-8fdf-c7447657c5f4)

# (ii) LU Decomposition of a matrix
![Screenshot 2025-04-24 220759](https://github.com/user-attachments/assets/6ca1784e-9b99-4fe9-869a-a7f456c1f046)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

