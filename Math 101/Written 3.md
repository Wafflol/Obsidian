2a.
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
b.
Evaluating the anti-derivative from the last question, we get
$$\int_{0}^{\pi} \sin(mx)\sin(nx) \, dx =\begin{bmatrix}
\frac{1}{m^2-n^2} (n\sin(mx)\cos(nx)-m\cos(mx)\sin(nx))
\end{bmatrix}_{0}^\pi$$
$$=\frac{1}{m^2-n^2}(n\sin(m\pi)\cos(n\pi)-m\cos(m\pi)\sin(n\pi)-(n\sin(0)\cos(0)-m\cos(0)\sin(0)))$$
$$= \frac{n\sin(m\pi)\cos(n\pi)-m\cos(m\pi)\sin(n\pi)}{m^2-n^2}$$
Because $m=n$, we can rewrite this 