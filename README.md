# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. read the elements of augmented matrix into array a and b
2. calculate elements of L and U
3. print L and U matrix
4. find V by solving LV=B by forword substitution
5. find X by solving UX = V by backward substitution
6. print array X as the solution

## Program:
(i) To find the L and U matrix
```python
'''Program to find L and U matrix using LU decomposition.
Developed by: JEECIKASRINA M
RegisterNumber: 23013947
'''
import numpy as np
from scipy.linalg import lu
A = np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```python
'''Program to solve a matrix using LU decomposition.
Developed by: JEECIKASRINA M
RegisterNumber: 23013947
'''
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A,B=eval(input()),eval(input())
lu,piv=lu_factor(A)
x = lu_solve((lu,piv),B)
print(x)
```
## Output:
(i) To find the L and U matrix.
![image](https://github.com/Jeecikasrina23013947/LU-Decomposition/assets/148515300/d7a2270f-f538-4fe0-a615-eb0a58202da2)

(ii) To find the LU Decomposition of a matrix.
![image](https://github.com/Jeecikasrina23013947/LU-Decomposition/assets/148515300/e21e7530-6368-4e99-bb60-ae29a975139e)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

