Starting with the generic formula for $\hbar (t)$, we get:
$$
\hbar (t) = \frac{1}{r}\int_{t-r}^{t} h(x) \, dx 
$$
thus, if we take the derivative of thus function, we end up with
$$
\hbar '(t) = \frac{1}{r} \frac{d}{dt}\int_{t-r}^{t} h(x) \, dx  
$$
$$
=\frac{1}{r} \frac{d}{dt} \begin{bmatrix}
h(t) - h(t-r)
\end{bmatrix}
$$
$$
=\frac{1}{r} (h'(t)-h'(t-r))
$$
Thus, by taking the value of the derivative at a point $t$, and subtracting it by the derivative of $h$ at a point $r$ away from $t$ and then dividing it by that distance, 