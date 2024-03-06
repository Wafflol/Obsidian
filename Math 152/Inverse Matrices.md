For a square matrix $A_{n\times m}$, if $\det A\neq 0$, then it is invertible and defines a one-to-one LT.

Matrix $B$ is called the inverse of $A$ iff $AB=BA=I$.

We use $A^{-1}$ to denote the inverse of $A$

#### How to find $A^{-1}$, given an invertible matrix $A$
Two methods:
##### Row operation/reduction
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
