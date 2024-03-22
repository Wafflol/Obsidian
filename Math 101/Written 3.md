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
Plugging $f(x)$ into the formula for $B_{n}(f)$, we get
$$B_{k}(f)=\frac{2}{\pi} \int_{0}^{\pi} f(x)\sin(nx) \, dx $$
$$=\frac{2}{\pi}\int_{0}^{\pi} (72\sin(x)+101\sin(2x)+108\sin(3x)+108\sin(4x)+111\sin(5x)) \sin(nx)\, dx $$
From the previous part, we see that if $n \neq m$, then the integral is equal to 0. Thus, we can split the previous integral into 5 integrals, where the coefficients of x match up in each sin:
$$\frac{2}{\pi}\int_{0}^{\pi} 72\sin^2x +101\sin^2(2x)+108\sin^2(3x)+108\sin^2(4x)+111\sin^2(5x)\, dx $$
Then, using the previous parts again, we know that the integral of each of the terms would be it's coefficient multiplied by $\frac{\pi}{2}$.
Thus, $\frac{\pi}{2}$ will cancel out with $\frac{2}{\pi}$, and thus the integral simplifies like so:
$$\frac{2}{\pi}* \frac{\pi}{2} * (72+101+108+108+111)$$
$$=500$$
Thus, $B_{n}(f) = 500$ for each integer $n \geq 1$

##### c. revised
Plugging f(x) into the formula for $B_{n}(f)$, we get
$$B_{k}(f)=\frac{2}{\pi}\int_{0}^{\pi} f(x)\sin(nx) \, dx $$
$$=\frac{2}{\pi}\int_{0}^{\pi} (72\sin(x)+101\sin(2x)+108\sin(3x)+108\sin(4x)+111\sin(5x)) \sin(nx)\, dx $$
From the previous part, we see that if $n\neq m$, then the integral is equal to 0. Thus, we know that at $n = 1$, all the terms except for the term with $72\sin(x)$ go to 0, giving us:
$$B_{1}(f) = \frac{2}{\pi}\int_{0}^{\pi} 72\sin^2x \, dx  $$
And from previous parts, we know that this integral will evaluate to 72. 
Thus, we can see that for $n = 2$,  the same thing will happen for the next term. And we can see that if $n> 5$, then the integral will evaluate to 0. 
##### d.
Since we know that for any integral $\int_{0}^{\pi} \sin(nx)\sin(mx) \, dx$, if $n\neq m$, then it evaluates to 0, then for an infinite series $f(x) = \sum_{k=1}^\infty b_{k}\sin(kx)$, $B_{k}f(x)$ at any specific $k$ would be equivalent to $\frac{2}{\pi}\int_{0}^{\pi} b_{k}\sin^2(kx) \, dx$. Thus, from the previous parts, we know that the integral evaluates to $b_{k}$. Therefore:
$$b_{n} = \frac{2}{\pi}\int_{0}^{\pi} f(x)\sin(nx) \, dx $$
for any $f(x) = \sum_{k=1}^\infty b_{k}\sin(kx)$.
