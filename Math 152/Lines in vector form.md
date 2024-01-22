Works in any dimension $\mathbb{R}^n$

Find eq. of line $L$ if one point on it and its direction are given.
Let $\vec{p} = (p_{1}, p_{2})$ be the point and $\vec{l} = (l_{1}, l_{2})$ be the direction.
Based on the graph, any point $\vec{x} = (x,y)$ on $L$ should satisfy:
$$
\vec{x} - \vec{p} = t\vec{l}
$$
1. Thus, the *point direction formula (parametric) is*
$$
\vec{x} = t\vec{l} + \vec{p}
$$
2. *Point-normal formula*
	 Find the equation line $L$ if one point on it and its normal direction are given.
	 $\vec{n} = (n_{1}, n_{2})$	
$$
\vec{n} \cdot (\vec{x} - \vec{p}) = 0
$$
Ex. write $y = 3x + 7$ in two vector forms
$$
1.\space \vec{x} = t\vec{l} + \vec{p} = t(1,3) + (0,7)
$$
$$
2.\space 0 = (3, -1) \cdot(x, (0,-7))
$$

$$
(3, -1)\cdot(x, y-7) =  3x - y + 7 = 0, \rightarrow y = 3x + 7
$$
When the equation of the line is written in the form, $3x - y = -7$, we know that $\vec{n}$  is $\begin{bmatrix}3 \\ -1\end{bmatrix}$
#### Point-normal formula of a line in $\mathbb{R}^3$
Given a point $\vec{p}$ and the normals $\vec{n_{1}}, \vec{n_{2}}$ of two [[Planes]] that intersect at the line,
$$
\begin{cases}
\vec{n_{1}}\cdot (\vec{x} - \vec{p}) = 0, \\
\vec{n_{2}}\cdot (\vec{x} - \vec{p}) = 0
\end{cases}
\space or \space 
\begin{cases}
\vec{n_{1}}\cdot \vec{x} = \vec{n_{1}}\cdot \vec{p}, \\
\vec{n_{2}}\cdot \vec{x} = \vec{n_{2}}\cdot \vec{p}
\end{cases}
$$
How to solve parametric equation of a line:
Ex. A line $L$ in $\mathbb{R}^3$ is defined by $\begin{cases}x+y+z=3\\x-y+2=-7\end{cases}$
Write equation of $L$ in parametric form:
$$
z = t
$$
$$
\begin{cases}
x+y+t=3 \\
x-y+2t=-7
\end{cases}
$$
$$
\begin{cases}
x+y=3-t \\
x-y=-7-2t
\end{cases}
$$
$$
(1) + (2) \Rightarrow 2x=-4-3t
$$
$$
x = -2-\frac{3}{2}t
$$
$$
x+y=-2-\frac{3}{2}t+y=3-t
$$
$$y= t+\frac{3}{2}t-t$$
$$
=5+\frac{1}{2}t
$$
$$
\vec{x} = \begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
= \begin{bmatrix}
-2-\frac{3}{2}t \\
5+\frac{1}{2}t \\
t
\end{bmatrix}
=\begin{bmatrix}
-2 \\
5 \\
0
\end{bmatrix}
+\begin{bmatrix}
-\frac{3}{2} \\
\frac{1}{2} \\
1
\end{bmatrix}
t
$$

[[Finding equation of two planes from a line L]]