For a 2x2 matrix:
$$
\begin{bmatrix}
a_{1} & a_{2} \\ b_{1} & b_{2}
\end{bmatrix}
$$
The determinant is simply $a_{1}b_{2}-a_{2}b_{1}$

For a 3x3 matrix:
$$
\begin{bmatrix}
a_{1} & a_{2} & a_{3} \\
b_{1} & b_{2} & b_{3} \\
c_{1} & c_{2} & c_{3}
\end{bmatrix}
$$
Multiply diagonals and add them up:
Left to right is positive, right to left is negative
Thus, the determinant for a 3x3 matrix is $a_{1}b_{2}c_{3}+b_{1}c_{2}a_{3}+c_{1}a_{2}b_{3}-a_{3}b_{2}c_{1}-b_{3}c_{2}a_{1}-c_{3}a_{2}b_{1}$

If there are many zeros in the determinant, it is easier to use the form 
$$
a_{1}\begin{vmatrix}
b_{2} & b_{3} \\
c_{2} & c_{3}
\end{vmatrix}
-a_{2}\begin{vmatrix}
b_{1} & b_{3} \\
c_{1} & c_{3}
\end{vmatrix}
+a_{3}\begin{vmatrix}
b_{1} & b_{2} \\
c_{1} & c_{2}
\end{vmatrix}
$$

#### For nxn matrices
$$\det A = \Sigma_{j_{1},j_{2},..j_{n}}(-1)^{j_{1}\dots jn}a_{1j_{1}}a_{2j_{2}}\dots a_{nj_{n}}$$
For a determinant, each term can only include one term from each column
For a [[triangular matrix]], due to this, the determinant is always the product of the diagonal entries, and the same applies for a [[diagonal matrix]]

The determinant is:
1. the sum of $n!$ terms
2. Each term is the product of $n$ entries containing only one from each row and each column

$$\det A = a_{i_{1}}c_{i_{1}}+a_{i_{2}}c_{i_{2}}+\dots+a_{in}c_{in}$$
$$A_{ij} = (i,j)th \text{ minor of }A$$
$$C_{ij} = (-1)^{i+j}\det A_{ij}$$
##### Properties:
1. $\det A = \det A^T$
2. Swapping a row makes it negative: $\det A_{k\leftrightarrow l} = -\det A$
3. If two rows are identical, the determinant is 0: $\det A_{k=l} = 0$
4. $\det(\alpha A) = \alpha^n\det A$
 