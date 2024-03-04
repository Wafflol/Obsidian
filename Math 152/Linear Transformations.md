To write a transformation as a matrix, $$M = \begin{bmatrix}

T(\vec{e_{1}}) & T(\vec{e_{2}})
\end{bmatrix}$$
Where $\vec{e_{1}}$ and $\vec{e_{2}}$ are the basis vectors

Can be thought of where the basis vectors end up after the transformation

To find a transformation matrix given 2 transformed vectors:
given $$T(\begin{bmatrix}
3 \\
2
\end{bmatrix}) = \begin{bmatrix}
1 \\
1
\end{bmatrix}, T(\begin{bmatrix}
2 \\
1
\end{bmatrix}) = \begin{bmatrix}
-1 \\
2
\end{bmatrix}$$
Express $e_{1}$ and $e_{2}$ as LCs of the two shown vectors.
$$\vec{x_{1}} = 3e_{1}+2e_{2}, \vec{x_{2}} = 2e_{1}+ e_{2}$$
$$\vec{e_{1}} = 2\vec{x_{2}}-\vec{x_{1}}, \vec{e_{2}}=2\vec{x_{1}}-3\vec{x_{2}}$$
Because it is linear, $$T(\vec{e_{1}}) = 2T(\vec{x_{2}})-T(\vec{x_{1}})$$
and the same for $T(\vec{e_{2}})$
