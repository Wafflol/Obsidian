A [[Linear Transformations|transformation]] $T: \mathbb{R}^n \to \mathbb{R}^m$ is followed by $S: \mathbb{R}^m\to \mathbb{R}^k$
The combined actions of the two is called a *composite* transformation denoted by $S(T(\vec{x}))$, or $S\circ T(\vec{x})$
$$M_{S \circ T} = M_{s}M_{t}$$
Ex.
$$T(\begin{bmatrix}
x_{1} \\
x_{2} \\
x_{3} \\
x_{4}
\end{bmatrix}) = \begin{bmatrix}
x_{1}-x_{2} \\
x_{2}-x_{3} \\
x_{3}-x_{4}
\end{bmatrix}$$
Find the transformation matrix:

$$M_{T} = \begin{bmatrix}
T(\vec{e_{1}}), T(\vec{e_{2}},\dots, T(\vec{n}))
\end{bmatrix}$$
$$= \begin{bmatrix}
1 & -1 & 0 & 0 \\
0 & 1 & -1 & 0 \\
0 & 0 & 1 & -1
\end{bmatrix}$$