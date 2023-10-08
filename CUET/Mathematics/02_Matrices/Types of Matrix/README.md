 #### 1. Column Matrix:
- A type of matrix that has only one column
- Example:

$$A = \begin{bmatrix} a_{1}\\  
a_{2}\\ 
a_{3} \\ 
..\\ 
a_{n}\end{bmatrix}$$


#### 2. Row Matrix:
- A type of matrix that has only one row.
- Example-

$$A = \begin{bmatrix} a_{1} & a_{2} & a_{3} & ... & a_{n}\end{bmatrix}$$


#### 3. Horizontal Matrix:
- A matrix in which the **number of columns is more that number of rows**.
- No. of Columns > No. of Rows.
- Example - 

$$A = \begin{bmatrix} a_{1,1} & a_{1,2}  & ... & a_{1,n} \\ 
a_{2,1} & a_{2,2} & ... & a_{2,n} \\ 
\end{bmatrix}$$


#### 4. Vertical Matrix: 
- A matrix in which the **number of rows is more that number of columns**.
- No. of Rows > No. of Columns.
- Example- 

$$A = \begin{bmatrix} a_{1,1} & a_{1,2}\\  
a_{2,1} & a_{2,2}\\ 
a_{3,1} & a_{3,2}\\  
a_{3,1} & a_{4,2}\\ 
a_{5,1} & a_{5,2}\end{bmatrix}$$


#### 5. Null Matrix:
- A matrix is said to be null matrix, **when all the elements of the that matrix is equals to zero**.
- Example-

$$A = \begin{bmatrix} 0 & 0 & 0 \\ 
0 & 0 & 0 \\ 
0 & 0 & 0\end{bmatrix}$$



#### 6. Square Matrix:
- A matrix in which the **number of rows and columns are same**.
- No. of Rows = No. of Columns.
- Example- 

$$A = \begin{bmatrix} a_{1,1} & a_{1,2}  & a_{1,3}\\  
a_{2,1} & a_{2,2}  & a_{2,3}\\ 
a_{3,1} & a_{3,2}  & a_{3,3} \end{bmatrix}$$

- The pair of elements $a_{ij}$ &  $a_{ji}$  are called **conjugate element**.
- The elements  $a_{1,1}$ $a_{2,2}$ $a_{3,3}$ ...... $a_{mm}$ are called **diagonal elements** also called **principal or leading diagonal**.
- Trace (A) = Sum of the elements of diagonal elements.
- $tr_{A} =$  $a_{1,1}$ + $a_{2,2}$  + $a_{3,3}$  + ...... +  $a_{mm}$.

#### Types of Square Matrix: 
- 
	#### 1. Triangular Matrix: 
	- If all elements above or below the leading/principle diagonal are zero in a square matrix, it is called triangular matrix
	- **Two types of traingular matrices are**
	1. Upper Triangular Matrix:
		- A square matrix whose all elements **below the leading diagonal is zero (i.e., aij = 0, I > j).**
		- Example-
		
$$A = \begin{bmatrix} 1 & 2 & 3 \\ 
0 & 5 & 6 \\ 
0 & 0 & 9 \\ 
\end{bmatrix}$$
		
2. Lower Triangular Matrix:
- A square matrix whose all elements **above the leading diagonal is zero (i.e., aij = 0, I < j).**
- Example-
		
$$ A = \begin{bmatrix} 1 & 0 & 0 \\ 
 4 & 5 & 0 \\ 
 7 & 8 & 9 \end{bmatrix}$$
		
	
#### 2. Diagonal Matrix:
- If all the elements of square matrix are **equals to zero except diagonal element**.
- Example-
	
$$A = \begin{bmatrix} d_{11} & 0 & 0 \\ 
 0 & d_{22} & 0 \\ 
 0 & 0 & d_{33} \\ \end{bmatrix}$$
	 
- Abbreviated as $dia(d_{11}, d_{22}, d_{33})$
- **Two types of Diagonal matrices are**
1. Scaler Matrix:
- If all the **diagonal elements of diagonal matrix are same**
- Example-
	 
$$A = \begin{bmatrix} 5 & 0 & 0 \\ 
 0 & 5 & 0 \\ 
 0 & 0 & 5 \\ \end{bmatrix}$$
		 
2. Unit Matrix:
	- Also known as Identity Matrix.
	- A diagonal matrix whose **all diagonal elements are equals to unit (or 1)**.
	- Example-
	
$$I_{3}\ =\ \begin{bmatrix} 1 & 0 & 0 \\ 
 0 & 1 & 0 \\ 
 0 & 0 & 1 \\ \end{bmatrix}\ I_{2}\ = \ \begin{bmatrix} 1 & 0\\ 
 0 & 1\end{bmatrix}$$
		 
- When a matrix is multiplied by a unit matrix, it remains same. $AI=A=IA$
 

#### 7. Orthogonal Matrix:
- The matrix is said to be an orthogonal matrix if the **product of a matrix and its transpose gives an identity value**.
- $A * A^{T} = I$.

#### 8. Symmetric Matrix:
- A matrix is called a symmetric matrix if **its transpose is equal to the matrix itself**.
- $A^{T} = A$.

$$A \ =\  A^{T}\  = \ \begin{bmatrix} 1 & 1 & -1 \\ 
1 & 2 & 0 \\ 
-1 & 0 & 5\end{bmatrix}$$
 
- #imp #note In every symmetric matrix the none principal diagonal element are look like mirror. i.e., $A_{i,j} = A_{j,i}$. #visualize

![symmetric visualize image](images/symmetricvisualize.png)

#### 9. Skew-Symmetric Matrix:
- A matrix is called a symmetric matrix if **its transpose is equal to the negative of matrix itself**.
- $A^{T} = -A$.

 $$A\ =\ \begin{bmatrix} 0 & 1 & -2 \\ 
-1 & 0 & 3 \\ 
2 & -3 & 0\end{bmatrix}\ A^{T}\ =\ -A\ =\ \begin{bmatrix} 0 & -1 & 2 \\
1 & 0 & -3 \\ 
-2 & 3 & 0\end{bmatrix}$$

- #imp #note Diagonal elements of Skew-Symmetric = 0 and none principal diagonal element have mirror image with opposite sign. #visualize 

![skew-symmetric visualize image](images/skew-symmetricvisualize.png)

#### 10. Harmition Matrix:
- A square matrix is said to hermition matrix, **if the transpose of its conjugate is equals to square matrix itself.**
- $A = (\bar{A})^{T}$ 
- Example-

![Harmition Matrix image](images/HarmitionMtrix.png)

#### 11. Skew-Harmition Matrix:
- A square matrix is said to skew-hermition matrix, **if the transpose of its conjugate is equals to negative of square matrix itself.**
- $A = -(\bar{A})^{T}$ 

#### 12. Unitary Matrix:
- A matrix is said to be unitary matrix, **when product of the It’s conjugate transpose with itself is equals to a unit matrix**.
- Represented by $A^{Q}$
- $A*A^{Q} = I$
- where, $A^{Q} = (\bar{A})^{T}$.

#### 13. Idempotent Matrix:               $A^{2} = A$

#### 14. Involutory Martix:               $A^{2} = I_{N}$

#### 15. Nilpotent Matrix:               $A^{k} = 0$

#### 16. Periodic Matrx:               $A^{k+1} = A$


