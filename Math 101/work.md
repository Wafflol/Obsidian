If $g(t) = \cos(\omega t)$, then we can use the formula from above to find $\bar{g}(t)$:
$$
\bar{g}(t) = \frac{1}{r}\int_{t-r}^{t} \cos(\omega x) \, dx = \frac{1}{r}\begin{bmatrix}
\frac{1}{\omega}\sin(\omega x)
\end{bmatrix}_{t-r}^t = \frac{1}{\omega r}(\sin(\omega t) - \sin(\omega (t-r))) = \frac{1}{\omega r}(\sin (\omega t) -\sin( \omega t-\omega r))
$$
We first start with the equation for part e:
$$
\bar{g}(t)= \frac{1}{\omega r}(\sin (\omega t) -\sin( \omega t-\omega r))
$$
distributing and then rewriting it using the sum identity, we get the following
$$
\bar{g}(t)=\frac{\sin (\omega t)}{\omega r} - \frac{\sin(\omega t-\omega r)}{\omega r}
$$
$$
=\frac{\sin(\omega t)}{\omega r}-\frac{\sin (\omega t)\cos(\omega r)-\cos(\omega t)\sin(\omega r)}{\omega r}
$$
Then, by taking the limit as r approaches 0, we can apply the small angle formulas, $\sin(\theta) = \theta$ and $\cos(\theta) = 1$ for a small angle $\theta$, and we get:
$$
\lim_{ r \to 0^+ }\bar{g}(t) =\frac{\sin(\omega t)}{\omega r}-\frac{\sin(\omega t)-\cos(\omega t)\omega r}{\omega r}
$$
$$
=\frac{\sin(\omega t)}{\omega r}-\frac{\sin(\omega t)}{\omega r}+\cos(\omega t)
$$
$$
=\cos(\omega t)
$$

