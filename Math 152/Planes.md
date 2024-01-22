#### The point normal formula of a plane in $\mathbb{R}^3$
Let $S$ be a plane in $\mathbb{R}^3$. Let $\vec{p}$ be a point on $S$ and $\vec{n}$ be its normal

Thus, the point normal formula of a plane is
$$
\vec{n}\cdot(\vec{x}-\vec{p}) = 0 \space or \space \vec{n}\cdot \vec{x} = \vec{n}\cdot \vec{p}
$$
Just like with [[Lines in vector form]], as $\vec{n} \cdot \vec{x} = \vec{n} \cdot \vec{p}$, if
$$
n_{1}x+n_{2}y+n_{3}z = \vec{n}\cdot \vec{p} = \alpha
$$
then,
$$
\vec{n} = (n_{1}, n_{2}, n_{3})
$$

#### Shortest distance from point $\vec{p}$ to plane $S$
To find the shortest distance from a point $\vec{p}$ to a plane $S$, simply find the normal $\vec{n}$ that passes through $\vec{p}$
Thus, we get 
$$
\vec{x} = t\vec{n} + \vec{p_{0}} \rightarrow \begin{bmatrix}
x \\
y \\
z \\
\end{bmatrix} = 
t\begin{bmatrix}
1 \\
-1 \\
1
\end{bmatrix}
+
\begin{bmatrix}
2 \\
0 \\
1
\end{bmatrix}
= 
\begin{bmatrix}
t+2 \\
-t \\
t+1
\end{bmatrix}
$$
Then, plug that into the plane equation, for ex. $x -y + z  = 6$:
$$
x - y + z = (t+2) - (-t) + (t+1) = 3t+3 = 6 \Rightarrow t = 1
$$
Thus, plugging it back into $\vec{x}$, we get
$$
\vec{x} = \begin{bmatrix}
3 \\
-1 \\
2 
\end{bmatrix}
$$
To find the distance between $\vec{x}$ and $\vec{p}$
$$
d = \begin{Vmatrix}
\vec{x_{0}} - \vec{p_{0}} \end{Vmatrix}
= \sqrt{ (3-2)^{2} + (-1)^{2} + (2-1)^{2}} = \sqrt{ 3 }
$$
#### Parametric formula of a plane in $\mathbb{R}^3$
Let $\vec{l_{1}}$, $\vec{l_{2}}$ be two linearly independent vectors and $\vec{p}$ be a point on plane $S$, then the parametric eq. of $S$ is given by
$$
\vec{x} - \vec{p} = \vec{s}l_{1} + \vec{t}l_{2}
$$
Alternatively,
$$
\vec{x} = \vec{p} + \vec{s}l_{1} + \vec{t}l_{2}
$$


##### Ex 2.8.6:
A plane $S$ is given in parametric form, find its point-normal formula
$$
\vec{x} = \begin{bmatrix}
1 \\
2 \\
1
\end{bmatrix}
+s\begin{bmatrix}
1 \\
0 \\
1
\end{bmatrix}
+t\begin{bmatrix}
1 \\
1 \\
0 
\end{bmatrix}

$$
Ans: The normal is
$$
\vec{n} = \vec{l_{1}} \vec{\times}l_{2} = \begin{vmatrix}
\hat{i} & \hat{j} & \hat{k} \\
1 & 0 & 1  \\
1 & 1 & 0
\end{vmatrix}
= (-1)\hat{i} - (-1)\hat{j} + \hat{k} = (-1, 1, 1)
$$
Thus,
$$
-x+y+z= -2
$$
##### Ex 2.8.7: *Preferred method*
A plane S is given by $x + 2y + 3z = 6$. Find one parametric formula of $S$
$$
\vec{n} = \begin{bmatrix}
1 \\
2 \\
3
\end{bmatrix}
$$
$$
x + 2y + 3z = 6
$$
$$
y = s, z = t
$$
$$
x + 2s + 3t = 6
$$
$$
x = 6 - 2s-3t
$$
$$
\vec{x} = \begin{bmatrix}
x \\
y \\
z \\

\end{bmatrix}
= \begin{bmatrix}
-6-2s-3t \\
s \\
t
\end{bmatrix}
= \begin{bmatrix}
6 \\
0 \\
0
\end{bmatrix}
+s\begin{bmatrix}
-2 \\
 1 \\
0
\end{bmatrix}
+t\begin{bmatrix}
-3 \\
0 \\
1
\end{bmatrix}
$$

Another way:
Find 3 points that satisfy the equation of the plane
Ex.
$$
x + 2y + 3z = 6
$$
$$
\vec{p_{0}} = \begin{bmatrix}
1 \\
1 \\
1
\end{bmatrix}
, \vec{p_{1}} = \begin{bmatrix}
6 \\
0 \\
0
\end{bmatrix}
, \vec{p_{2}} = \begin{bmatrix}
0 \\
0 \\
2
\end{bmatrix}

$$
Now, let
$$
\vec{l_{1}} = \vec{p_{1}} - \vec{p_{0}} = \begin{bmatrix}
5 \\
-1 \\
-1
\end{bmatrix}, 
\vec{l_{2}} = \vec{p_{2}} - \vec{p_{0}} = \begin{bmatrix}
-1 \\
-1 \\
1
\end{bmatrix}
$$
$$
\vec{x} = \vec{p_{1}} + \vec{s}l_{1} + \vec{t}l_{2} = \begin{bmatrix}
6 \\
0 \\
0
\end{bmatrix}
+s\begin{bmatrix}
5 \\
-1 \\
-1
\end{bmatrix}
+t\begin{bmatrix}
-1 \\
-1 \\
1
\end{bmatrix}
$$
[[Projection onto a plane]]