##### 2a.
Taking the derivative using chain rule and product rule, we get:
$$\frac{d}{dx}\begin{bmatrix}
K\sin(mx)\cos(nx)+D\cos(mx)\sin(nx)
\end{bmatrix}$$
$$=K(\cos(mx)m\cos(nx)-\sin(mx)\sin (nx)n)+D(\cos(nx)n\cos(mx)-\sin(mx)m\sin(nx))$$
$$=K(m\cos(mx)\cos(nx)-n\sin(mx)\sin(nx))+D(n\cos(nx)\cos(mx)-m\sin(mx)\sin(nx))$$
We want to cancel out the $\cos$ terms. Thus, they need to have equal and opposite coefficients, so we can use $K = n$ and $D = -m$ to make the terms cancel out:
$$K = n, D = -m$$
$$nm\cos(mx)\cos(nx)-n^2\sin(mx)\sin(nx)-mn\cos(mx)\cos(nx)+m^2\sin(mx)\sin(nx)$$
$$=(m^2-n^2)\sin(mx)\sin(nx)$$
Thus, we can see that the derivative  $\frac{d}{dx}f(x) =(m^2-n^2)\sin(mx)\sin(nx)$. Thus, we can see that it only differs from $\sin(mx)\sin(nx)$ by a constant. Therefore, the anti-derivative  is simple:
$$\int f(x) \, dx = \frac{1}{m^2-n^2} (n\sin(mx)\cos(nx)-m\cos(mx)\sin(nx))+C$$
##### b.
As $m = n$, we can rewrite the integral as:
$$\int_{0}^{\pi} \sin^2(mx) \, dx $$
solving this integral, we get:
$$\int_{0}^{\pi} \frac{1-\cos(2mx)}{2} \, dx $$
$$=\begin{bmatrix}
\frac{1}{2}x-\frac{\sin(2mx)}{2m}
\end{bmatrix}_{0}^\pi$$
$$= \frac{1}{2}(\pi)-\frac{\sin(2\pi m)}{2m}-\left( \frac{1}{2}(0)-\frac{\sin(0)}{2m} \right)$$
As $m$ is a positive integer, and $\sin$ of any multiple of $2\pi$ is 0, we can see that the definite integral evaluates to $\frac{\pi}{2}$, and thus, $R=\frac{\pi}{2}$

##### c.
Plugging $f(x)$ into the formula for $B_{n}(f)$, we get:
