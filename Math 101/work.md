Starting by rewriting $F(s)$ as a series of simple integrals, as we can see from the graph, the graph oscillates between the values 0 and 1 every integer. Thus, as we know that $F(s) = \int_{0}^{\infty} e^{-st}f(t) \, dt$, we can rewrite $F(s)$ as a series of integrals that alternates between 0 and 
$$F(s) = \sum_{n=0}^\infty \int_{n}^{n+1} \left(1-1^n \right) (e^{-st})\, dt $$
$$F(s) = \sum_{n=0}^\infty \begin{bmatrix}
\frac{1-1^n}{-se^{st}}
\end{bmatrix}^{n+1}_{n}$$
$$= \sum_{n=0}^\infty\frac{1-1^{n}}{-se^{s(n+1)}}+\frac{1-1^n}{se^{sn}}$$
$$=\sum_{n=0}^\infty (1-1^n) \left( \frac{e^s}{se^{sn+s}}- \frac{1}{se^{sn+s}} \right)$$
If we manipulate the series to take out where the function is equal to 0, we get:
$$F(s) = \sum_{n=0}^\infty \frac{e^s-1}{se^{2sn+s}}$$

Knowing that $f(t) = 0$ for every other integer interval, we can write $F(s)$ as an infinite series of integrals:
$$F(s) = \int_{0}^{1} e^{-st} \, dt  + \int_{2}^{3} e^{-st} \, dt + \int_{4}^{5} e^{-st} \, dt +\dots + \int_{n}^{n+1} e^{-st} \, dt $$
Evaluating the anti-derivative for $\int e^{-st} \, dt$, we get:
$$\int e^{-st} \, dt  = -\frac{1}{se^{st}}+C$$
And now, plugging this into $F(s)$,
$$F(s) = -\frac{1}{se^s}+\frac{1}{s}-\frac{1}{se^{3s}}+\frac{1}{se^{2s}}-\frac{1}{se^{5s}}+\frac{1}{se^{4s}}+\dots-\frac{1}{se^{(n+1)s}}+\frac{1}{se^{ns}}$$
