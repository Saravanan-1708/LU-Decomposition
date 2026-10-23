# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5.End of the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: saravanan R
RegisterNumber: 26008206
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P, L, U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: saravanan R
RegisterNumber: 26008206
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:
![lu decomposition]()
<img width="1322" height="851" alt="Screenshot 2026-10-23 085616" src="https://github.com/user-attachments/assets/13978732-d5b6-4217-beaa-72b0227ae515" />
<img width="1311" height="847" alt="Screenshot 2026-10-23 085740" src="https://github.com/user-attachments/assets/65069ab2-fac4-427b-8a41-24425d238faa" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

