#### Row Echelon Form (REF)
1. rewrite with an augmented matrix
2. use elimination to solve

Ex. in case one is a linear combination of the other 2
$$
\begin{bmatrix}
 1 & 1 & 1 & | & 1\\
1 & 2 & 3 & | & 1 \\
2 & 3 & 4 & | & 2
\end{bmatrix}
$$
$$
=\begin{bmatrix}
1 & 1 & 1 & | & 1 \\
0 & 1 & 2 & | & 0 \\
0 & 0 & 0 & | & 0
\end{bmatrix}
$$
if last row is all 0, sub in t for $x_{3}$
Thus,
$$
\vec{x} = \begin{bmatrix}
x_{1} \\
x_{2} \\
x_{3}
\end{bmatrix}
=\begin{bmatrix}
1+t \\
-2t \\
t
\end{bmatrix}
=t\begin{bmatrix}
1 \\
-2 \\
1
\end{bmatrix}
+\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$$
The solution is thus a line

Applications of GE:

Checking for [[Linear indenpendence]]
