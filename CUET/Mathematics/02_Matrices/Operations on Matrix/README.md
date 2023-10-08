## Transpose of Matrix
- The transpose of the matrix can be found **by interchanging rows and columns**.
- Denoted by $A^{T}$.
 
$$A = \begin{bmatrix} a & b & c \\ 
 d & e & f \end{bmatrix}_{2 X 3}\ \ \  A^{T}\ =\ \begin{bmatrix} a & d \\ 
 b & e \\ 
 c & f \end{bmatrix}_{3 x 2}$$
   

## Adjoint of Matrix
- The adjoint of the matrix can be defined **as the transpose of the cofactor of that particular matrix**.
- $Adjoint = (Cofactor)^{T}$
- Denoted by $adj.A$.
- Here positive and negative sign depends upon the sum of the indices of the matrix if the sum is an odd number, then sign will be negative else remains positive.

![adjoint property image](images/adjointproperty.png)

## Inverse of Matrix
- Inverse matrix is obtained **by dividing the adjugate of the given matrix by the determinant of the given matrix**.
- Denoted by $A^{-1}$ .

$$\begin{equation*} A^{-1} = \frac{1}{|A|} * adj.A \end{equation*}$$

- #note $A^{-1}$ exists if A is a non-singular. i.e., $|A| \neq 0$.
- #imp #shortcut #trick #inverseMatrix
1. Shortcut for Matrix of order $2 * 2$  
		 
$$A = \begin{bmatrix} a & b \\ 
c & d \end{bmatrix} \Longrightarrow A^{-1} = \frac{1}{|A|} * \begin{bmatrix} d & -c \\ 
-b & a \end{bmatrix}$$

2. Shortcut for Diagonal Matrix.  
 
$$A = \begin{bmatrix} 1 & 0 & 0 \\ 
0 & 2 & 0 \\ 
0 & 0 & 3 \end{bmatrix}\ \Longrightarrow\ A^{-1}\ =\ \frac{1}{|A|}\ *\ \begin{bmatrix}\ \frac{1}{1} & 0 & 0 \\ 
0 & \frac{1}{2} & 0 \\ 
0 & 0 &\frac{1}{3} \end{bmatrix}$$
		
- **Properties of Inverse Matrix**
![inverseProperty image](images/inverseProperty.png)

