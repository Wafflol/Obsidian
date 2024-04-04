Starting by rewriting $F(s)$ as a series of simple integrals, as we can see from the graph, the graph oscillates between the values 0 and 1 every integer. Thus, as we know that $F(s) = \int_{0}^{\infty} e^{-st}f(t) \, dt$, we can rewrite $F(s)$ as a series of integrals that alternates between 0 and 
$$F(s) = \sum_{n=0}^\infty \int_{n}^{n+1} \left(1-1^n \right) (e^{-st})\, dt $$
$$F(s) = \sum_{n=0}^\infty \begin{bmatrix}
\frac{1-1^n}{-se^{st}}
\end{bmatrix}^{n+1}_{n}$$
$$= \frac{1-1^{n}}{-se^{s(n+1)}}+\frac{1-1^n}{se^{sn}}$$
