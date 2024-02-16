Let $A_{m\times k}$, $B_{q\times n}$ be of sizes $m\times k, q\times n$, then
$$C_{m\times n} = A_{m\times k}B_{q\times n}$$
if $k = q$

Multiplying a matrix $A$ by an identity matrix $I$ = $IA$ = $A$

Any [[Solving a linear system| linear system]] can be written as a matrix
where 
$$A = \begin{bmatrix}
a_{11} & \dots & a_{1n} \\
\dots & \dots & \dots \\
a_{m_{1}} & \dots & a_{mn} \\
\end{bmatrix}, \vec{x} = \begin{bmatrix}
x_{1} \\
\dots \\
x_{n}
\end{bmatrix}, \vec{b} = \begin{bmatrix}
b_{1} \\
\dots \\
b_{m}
\end{bmatrix}$$

When $A_{n\times n}$ is square, there is a strong resemblance between $ax = b$ and $A\vec{x} = \vec{b}$

| Cases | $ax = b$ | $A\vec{x} = \vec{b}$ |
| ---- | ---- | ---- |
| Unique solution | If $a\neq 0$, $x = a^{-1}b$ | If $\|A\| \neq 0$, $\vec{x} = A^{-1}\vec{b}, A^{-1}$ is the inverse of $A$ |

For a [[triangular matrix]], or a [[diagonal matrix]] $A$, where $A = \begin{bmatrix}a&b\\c&d\end{bmatrix}$, 
$$A^2 = \begin{bmatrix}
a^2 & b^2 \\
c^2 & d^2
\end{bmatrix}$$
