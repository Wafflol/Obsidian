To find $\bar{f}_{0}, \bar{f}_{1}, \bar{f}_{2}$, we can just plug it into the equation given above
$$
\bar{f}_{0}(t)=\frac{1}{r}\int_{t-r}^{t} 1 \, dx = \frac{1}{r}\begin{bmatrix}
t
\end{bmatrix}_{t-r}^t = \frac{1}{r}(t-(t-r)) = 1 
$$
$$
\bar{f}_{1}(t) = \frac{1}{r}\int_{t-r}^{t} x \, dx = \frac{1}{r}\begin{bmatrix}
\frac{1}{2}x^2
\end{bmatrix}_{t-r}^t  = \frac{1}{r}\left( \frac{1}{2}t^2 -\frac{1}{2}(t-r)^2\right) = \frac{1}{r}\left( \frac{1}{2}t^2 - \frac{1}{2}(t^2-2tr+r^2)\right) = \frac{1}{r}(2tr-r^2) = 2t-r
$$
$$
\bar{f}_{2}(t) = \frac{1}{r}\int_{t-r}^{r} x^2 \, dx = \frac{1}{r}\begin{bmatrix}
\frac{1}{3}x^3
\end{bmatrix}_{t-r}^r = \frac{1}{r}\left( \frac{1}{3}r^3-\frac{1}{3}(t-r)^3 \right)
$$

