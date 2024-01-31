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

#### Homogeneous systems
Has the form $A\vec{x} = 0$
Looks like
$$
\begin{bmatrix}
x & x & x & | & 0 \\ 
x & x & x & | & 0 \\ 
x & x & x & | & 0 
\end{bmatrix}
$$
#### Non-homogeneous systems
Form $A\vec{x} = \vec{b}$


Ex. Given two lines $\vec{x} = \begin{bmatrix}9+t\\11+2t\\12-2t\end{bmatrix}, \vec{x} = \begin{bmatrix}9-s\\17-4s\\s+p\end{bmatrix}$
where $s, t$ are parameters, $p$ is a scalar to be determined
a. for $p=?$, $L_{1}$ and $L_{2}$ intersect with each other
Set them equal to each other and rearrange:
$$
\begin{bmatrix}
s+t \\
4s+2t \\
-s-2t
\end{bmatrix}
=\begin{bmatrix}
0 \\
6 \\
p-12
\end{bmatrix}
$$
$$
\begin{bmatrix}
1 & 1 & | & 0 \\
4 & 2 & | & 6 \\
-1 & -2 & | & p-12
\end{bmatrix}
$$
Do REF:
$$
\begin{bmatrix}
1 & 1 & | & 0 \\
0 & 1 & | & -3 \\
0 & 1 & | & 12-p
\end{bmatrix}
$$
$$
\begin{bmatrix}
1 & 1 & | & 0 \\
0 & 1 & | & -3 \\
0 & 0 & | & 15-p
\end{bmatrix}
$$
$L_{1}$ and $L_{2}$ intersect if $p = 15$
otherwise they do not intersect


#### Challenging example
Find the shortest distance between two lines:
$$
L_{1}: \vec{x} = \begin{bmatrix}
1  \\
1 \\
1
\end{bmatrix}

$$
$$
L_{2}: \vec{x} = t\begin{bmatrix}
1 \\
2 \\
3
\end{bmatrix}
+\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix}
$$
