### A matrix is a rectangular _array of numbers_ (or other mathematical objects)
##### General Matrix
$$\begin{bmatrix} a_{1,1} & a_{1,2}  & ... & a_{1,n} \\  
a_{2,1} & a_{2,2} & ... & a_{2,n} \\ 
a_{3,1} & a_{3,2} & ... & a_{3,n} \\ 
.. & .. & .. & ...  \\ 
a_{m,1} & a_{m,2} & .. & a_{m,n}\end{bmatrix}$$

### Special Matrix       #imp #specialMatrix
1. If there is a matrix, like

$$A = \begin{bmatrix}  cos\alpha & -sin\alpha \\
sin\alpha & cos\alpha \end{bmatrix}$$
	
the the $A^{N}$, will be
	
$$A^{N} = \begin{bmatrix}  cos(N\alpha) & -sin(N\alpha) \\
sin(N\alpha) & cos(N\alpha) \end{bmatrix}$$


2. If there is a matrix, like
	
$$A = \begin{bmatrix} 1 & n \\
 0 & 1 \end{bmatrix}$$
	 
then
	
$$A = \begin{bmatrix} 1 & n_{1} \\
 0 & 1 \end{bmatrix} * \begin{bmatrix} 1 & n_{2} \\ 
 0 & 1 \end{bmatrix} = \begin{bmatrix} 1 & (n_{1}+n_{2}) \\ 
 0 & 1 \end{bmatrix}$$
	 
3. If there is a matrix, like
	
$$A = \begin{bmatrix} 1 & 0 & 0 \\ 
0 & 1 & 1 \\ 
1 & 0 & 0 \end{bmatrix}$$    

then, 

$$A^{2} = \begin{bmatrix} 1 & 0 & 0 \\ 
1 & 1 & 1 \\ 
1 & 0 & 0 \end{bmatrix} \ A^{3} = \begin{bmatrix} 1 & 0 & 0 \\ 
2 & 1 & 1 \\ 1 & 0 & 0 \end{bmatrix} \ A^{4} = \begin{bmatrix} 1 & 0 & 0 \\
3 & 1 & 1 \\
1 & 0 & 0 \end{bmatrix} \  A^{n} = \begin{bmatrix} 1 & 0 & 0 \\
n-1 & 1 & 1 \\ 
1 & 0 & 0 \end{bmatrix}$$

4. If there is a matrix, like
	
$$A = \begin{bmatrix} 1 & 0 \\ 
1/2 & 1 \end{bmatrix}$$    

then, 

$$A^{2} = \begin{bmatrix} 1 & 0 \\ 
2/2 & 1 \end{bmatrix} \ A^{3} = \begin{bmatrix} 1 & 0 \\ 
3/2 & 1 \end{bmatrix} \ $A^{4} = \begin{bmatrix} 1 & 0 \\ 
4/2 & 1 \end{bmatrix} \ A^{n} =  \begin{bmatrix} 1 & 0 \\ 
n/2 & 1 \end{bmatrix}$$
	
#tip #note **Whenever you get any question to find the big big power of any Matrix $\to$ find its power of 2 & 3, you will catch the special about that matrix is changing relatively.
i.e., Find $A^{n} \to A^{2} A^{3}  \to$ speciality appears.** 

If $\omega$ is a complesx cube root of unity, then:
- $1 + \omega+\omega^2 = 0$
- $\omega^3 = 1$


![[02_Matrices/Operations on Matrix/README]]

![[02_Matrices/Types of Matrix/README]]