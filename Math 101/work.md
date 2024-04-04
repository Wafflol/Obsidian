Starting by rewriting $F(s)$ as a series of simple integrals, as we can see from the graph, the graph oscillates between the values 0 and 1 every integer. Thus, as we know that $F(s) = \int_{0}^{\infty} e^{-st}f(t) \, dt$, we can rewrite $F(s)$ as a series of integrals that alternates between 0 and 
$$F(s) = \sum_{n=0}^\infty \int_{n}^{n+1} \left(1-1^n \right) (e^{-st})\, dt $$


$$F(s) = \sum_{n=0}^{\infty}\int_{0}^{\infty} \left(  \frac{1}{2} +\frac{1}{2}(-1)^n \right) * e^{-st} \, dt $$
$$= \sum_{n=0}^{\infty}\lim_{ a \to \infty } \int_{0}^{a} \left( \frac{1}{2}e^{-st} \right)(1-1^n) \, dt $$
$$= \sum_{n=0}^{\infty}\lim_{ a \to \infty } [-\frac{1}{2s}e^{-st}(1-1^n)]_{0}^a$$
$$= \sum_{n=0}^{\infty}\left( \lim_{ a \to \infty } \left( -\frac{1}{2s}e^{-sa}(1-1^n)-\left( -\frac{1}{2s}(1-1^n) \right) \right) \right)$$
$$= \sum_{n=0}^{\infty} \frac{1-1^n}{2s}$$