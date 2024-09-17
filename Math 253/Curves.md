In $\mathbb{R}^2$
$$\gamma: I < \mathbb{R} \to \mathbb{R}^2$$
In $\mathbb{R}^3$
$$\gamma(t) = (x(t),y(t),z(t))$$
$$\gamma: I \leq \mathbb{R} \to (x(t),y(t),z(t)) \in \mathbb{R}^3$$

**Examples**
1.
lines in 3d
![[Pasted image 20240916110921.png]]
**injective**

2.
Circles in 2d
$$t \in [0,2\pi]$$
$$x(t) = R\cos t$$
$$y(t) = R\sin t$$
3.
Circles in 3d
$$\begin{cases}
x(t) = x_{0} + R\cos t \\
y(t) = y_{0} + R\sin t \\
z(t) = z_{0}
\end{cases}$$
![[Pasted image 20240916111938.png]]

Remark: for any $\gamma$ we can construct 
$$\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j} + z(t)\hat{k}$$

$$\hat{l}, \hat{m}, \hat{n} = \text{orthogonal vectors}$$
$$\hat{r}(t)=\vec{x}(t)\hat{l}+\vec{y}(t)\hat{m}+\vec{z}(t)\hat{n}$$
Example (Circle in 3D)
$$\vec{r}_{1}(t)=R\cos (t)\hat{i}+R\sin (t)\hat{j}+\hat{k}$$
$$\hat{i} = <1,0,0>, \hat{j} = <0,1,0>, \hat{k} = <0,0,1>$$
Consider
$$\hat{l}= \begin{bmatrix}
0 \\
\frac{1}{\sqrt{ 2 }} \\
-\frac{1}{\sqrt{ 2 }}
\end{bmatrix},\hat{m}=\begin{bmatrix}
0 \\
-\frac{1}{\sqrt{ 2 }} \\
\frac{1}{\sqrt{ 2 }}
\end{bmatrix}, \hat{n} = \begin{bmatrix}
1 \\
0 \\
0 
\end{bmatrix}$$
$$\hat{n}\cdot \hat{m} = 0$$
$$\hat{l} \cdot \hat{m} = 0$$
_____

Circle 2
$$r_{2}(t) = R\cos t \cdot \hat{l} + R\sin t\cdot \hat{m} + 1\cdot \hat{n}$$
$$(x_{1}(t)=\vec{x}(t),y(t)=\vec{y}(t),z(t)=\vec{z}(t))$$
$$\begin{cases}
x_{2}(t) = 1\\
y_{2}(t) =  \frac{R\cos t-R\sin t}{\sqrt{ 2 }}\\
z_{3}(t) = \frac{-R\cos t-R\sin t}{\sqrt{ 2 }} 
\end{cases}$$

$$(x_{2}(t),y_{2}(t),z_{2}(t)) \text{ always refers to the standard coordinates}$$
