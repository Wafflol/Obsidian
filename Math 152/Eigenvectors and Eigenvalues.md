For an $n\times n$ transformation matrix $A$, a vector $\vec{v}$ and a scalar $\lambda$ are called an eigen-pair of $A$ for:
$$\vec{v} \neq 0$$
$$A\vec{v}=\lambda \vec{v}$$
$\vec{v}$ is the eigenvector, and $\lambda$ is the eigenvalue

Eigenvectors are never 0, but eigenvalues can be

For an $n\times n$ matrix, often there exist $n$ eigen-pairs, especially when no repeated eigenvalues occur

To calculate eigen-pairs:
We need to find a homogeneous solution for $A\vec{v}=\lambda \vec{v}$
$$(A-\lambda I)\vec{v}=0$$
$$\det(A-\lambda I) = 0$$
$$=\lambda^2-Tr\lambda+\det$$
Where Tr is the [[Trace|trace]]

Factoring this out:
$$(\lambda-\lambda_{1})(\lambda-\lambda_{2})=0$$
$$Tr = \lambda_{1}+\lambda_{2}$$
$$Det = \lambda_{1}\lambda_{2}$$

Thus, for any $2\times 2$ matrix, the [[Characteristic equation]] (polynomial) is:
$$\lambda^2-Tr\lambda+Det=0$$

##### Eg. 6.2.11 Find all eigen-pairs of
$$A = \begin{bmatrix}
-9 & -2 & 6 \\
4 & -3 & -6 \\
-6 & -3 & 2
\end{bmatrix}$$
$$\begin{vmatrix}
A - \lambda I
\end{vmatrix} = 0 = \begin{vmatrix}
-9-\lambda & -2 & 6 \\
4 & -3-\lambda & -6 \\
-6 & -3 & 2-\lambda
\end{vmatrix}$$
$$(1) = (1) + (2)$$
$$\begin{vmatrix}
-5-\lambda & -5-\lambda & 0 \\
4 & -3-\lambda & -6 \\
-6 & -3 & 2-\lambda
\end{vmatrix}$$
factor out $-\lambda-5$
$$-(\lambda+5)\begin{vmatrix}
1 & 1 & 0 \\
4 & -3-\lambda & -6 \\
-6 & -3 & 2-\lambda
\end{vmatrix}$$
$$-(\lambda+5)(\begin{vmatrix}
-3-\lambda & -6 \\
-3 & 2-\lambda
\end{vmatrix} - \begin{vmatrix}
4 & -6 \\
-6 & 2-\lambda
\end{vmatrix}) $$
$$-(\lambda+5)(\lambda^2+\lambda-6-18+4\lambda-8+36)$$
$$-(\lambda+5)(\lambda^2+5\lambda+4)$$
$$=-(\lambda+5)(\lambda+1)(\lambda+4)$$
$$\lambda_{1} = -1, \lambda_{2} = -4, \lambda_{3} = -5$$
For $\lambda_{1} = -1$
$$A - \lambda_{1}I = A+I$$
$$ker\begin{bmatrix}
-8 & -2 & 6 \\
4 & -2 & -6 \\
-6 & -3 & 3
\end{bmatrix}$$
$$= \begin{bmatrix}
1 \\
-1 \\
1
\end{bmatrix}$$
For $\lambda_{2} = -4$
$$A - \lambda_{2}I = A + 4I$$
$$ker\begin{bmatrix}
-5 & -2 & 6 \\
4 & 1 & -6 \\
-6 & -3 & 6
\end{bmatrix}$$
$$= \begin{bmatrix}
2 \\
-2 \\
1
\end{bmatrix}$$
For $\lambda_{3} = -5$
$$A - \lambda_{3}I = A+5I$$
$$ker\begin{bmatrix} 
-4 & -2 & 6 \\
4 & 2 & -6 \\
-6 & -3 & 7
\end{bmatrix}$$
$$= \begin{bmatrix}
1 \\
-2 \\
0
\end{bmatrix}$$

##### Eg. 6.2.12 Repeated Eigenvalues
Find all eigen-pairs of $A = \begin{bmatrix}2&1\\0&2\end{bmatrix}$
[[Algebraic Multiplicity]] (AM) is defined as the number of times the same eigenvalue occurs as a root of the characteristic equation $\det(A-\lambda I) = 0$ 
$$(AM) = 2$$
$$ker(A-2I) = ker\begin{bmatrix}
0 & 1 \\
0  & 0
\end{bmatrix} = \begin{bmatrix}
1 \\
0
\end{bmatrix}$$
Eg. 6.2.13 Repeated eigenvalue without "missing" eigenvector
$$A = \begin{bmatrix}
2 & 1 & 0 \\
0 & -1 & 0 \\
0 & -1 & 2
\end{bmatrix}$$
$$\lambda_{1} = -1, \lambda_{2}=\lambda_{3}=2$$
$$\lambda_{1}=-1, ker(A+I) = \begin{bmatrix}
1 \\
-3 \\
-1
\end{bmatrix}$$
$$\lambda_{2} = 2, ker(A-2I) = ker\begin{bmatrix}
0 & 1 & 0 \\
0 & -3 & 0 \\
0 & -1 & 0
\end{bmatrix}$$
$$\vec{v_{1}} = \begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}, \vec{v_{2}} = \begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}$$