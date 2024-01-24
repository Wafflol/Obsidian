Consider a system of 3 linear eq.
$$
\begin{cases}
a_{11}x+a_{12}y+a_{13}z=b_{1} \\
a_{21}x+a_{22}y+a_{23}z=b_{2} \\
a_{31}x+a_{32}y+a_{33}z=b_{3}
\end{cases}
$$
where $a_{ij}$, $b_{i}$, ($i, j$ = 1, 2, 3) are scalars in $\mathbb{R}$

Each eqn defines a plane in $\mathbb{R}^3$
There are 3 possible situations:
![[Jan 24 Linear independence.png]]
#### Linear Dependence vs Linear Independence
Two vectors are linearly dependent if they are parallel to each other
If the two vectors are not parallel, they are linearly independent

There are at most 2 LI vectors in $\mathbb{R}^2$

#### How to check for linear independence
If the determinant of the set of vectors $\neq 0$, the vectors are linearly independent
If one vector is a scalar multiple of the other, then the two vectors are linearly dependent

#### Summary
In $\mathbb{R}^2$, 2 vectors are LI if they point to different directions
In $\mathbb{R}^3$, 3 vectors pointing to 3 different directions can not guarantee that they are LI. They are Li only when they are NOT in the same plane
In $\mathbb{R}^n$, $n$ vectors are LI iff none of them can be expressed as a nontrivial LC of the others/ Or when the volume of the "hyper-parallelepiped" with sides defined by these vectors is nonzero (using the determinant of the $n\times n$ matrix)