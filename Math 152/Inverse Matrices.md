For a square matrix $A_{n\times m}$, if $\det A\neq 0$, then it is invertible and defines a one-to-one LT.

Matrix $B$ is called the inverse of $A$ iff $AB=BA=I$.

We use $A^{-1}$ to denote the inverse of $A$

#### How to find $A^{-1}$, given an invertible matrix $A$
Two methods:
##### Row operation/reduction (see [[RREF]])
If $A$ is invertible, then finding the inverse is equivalent to solving $A\vec{x} = \vec{y}$ for $\vec{x}$

$$A\vec{x} = I\vec{y}, I\vec{x} = A^{-1}\vec{y}$$
Solved by using $$\begin{bmatrix}
A & | & I
\end{bmatrix}$$
where RREF gives:
$$\begin{bmatrix}
I & | & A^{-1}
\end{bmatrix}$$
Ex.
Find inverse of A = $\begin{bmatrix}1&4\\2&7\end{bmatrix}$
$$\begin{bmatrix}
1 & 4 & | & 1 & 0 \\
2 & 7 & | & 0 & 1
\end{bmatrix}$$
$$R_{2}=R_{2}-2R_{1}$$
$$\begin{bmatrix}
1 & 4 & | & 1 & 0  \\
0 & -1 & | & -2 & 1
\end{bmatrix}$$
$$R_{1} = R_{1}+4R_{2}$$
$$\begin{bmatrix}
1 & 0 & | & -7 & 4 \\
0 & 1 & | & 2 & -1
\end{bmatrix}$$
Check answer:
$$\begin{bmatrix}
-7 & 4  \\
2 & -1
\end{bmatrix}
\begin{bmatrix}
1 & 4 \\
2 & 7
\end{bmatrix}
=\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}$$
$$A^{-1} = \begin{bmatrix}
-7 & 4 \\
2 & -1
\end{bmatrix}$$
##### Solved using formula
$$A^{-1} = \frac{1}{\det A}\begin{bmatrix}
d & -b \\
-c & a
\end{bmatrix}$$

#### Properties of matrix inverse
1. if $A$ is invertible, then $A^{-1}$ exists and is unique
2. If $A, B$ are both invertible, so is $AB$ and that $(AB)^{-1}$ = $B^{-1}A^{-1}$
3. If $A$ is invertible, then $A\vec{x} = \vec{b} \iff \vec{x} = A^{_-1}\vec{b}$
![[Pasted image 20240306125031.png]]