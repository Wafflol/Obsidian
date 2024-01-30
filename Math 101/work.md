Starting with the generic formula for $\bar{h} (t)$, we get:
$$
\bar{h} (t) = \frac{1}{r}\int_{t-r}^{t} h(x) \, dx 
$$
thus, if we take the derivative of this function, we end up with 
$$
\bar{h} '(t) = \frac{1}{r} \frac{d}{dt}\int_{t-r}^{t} h(x) \, dx  
$$
$$
=\frac{1}{r} \frac{d}{dt} \begin{bmatrix}
H(t) - H(t-r)
\end{bmatrix}
$$
, where $H(t)$ is the anti-derivative of $h(t)$.
Then, after simplifying, we get the following equation:
$$
=\frac{1}{r} (h(t)-h(t-r))
$$
Thus, this equation takes on the form of the equation of a slope, with the function being $h(t)$, from the point $t-r$ to $t$.
