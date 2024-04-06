Because we know that the first two terms of $\hat{T}_{N-2}$ match the first two terms of $T_{N-2}$, the series for $T_{N-2}, S_{N}, S_{N-1}, S_{N-2}$ can be written out like so:
$$T_{N-2} = \sum_{n=(N-2)+1}^\infty = a_{n} = a_{N-1}+a_{N} + a_{N+1}+\dots$$
$$S_{N} = \sum_{n=1}^N = a_{n} = a_{1}+a_{2} +\dots+ a_{N-1}+a_{N}$$
$$S_{N-1} = \sum_{n=1}^{N-1} = a_{n} = a_{1}+a_{2} +\dots+ a_{N-2}+a_{N-1}$$
$$S_{N-2} = \sum_{n=1}^{N-2} = a_{n} = a_{1}+a_{2} +\dots+ a_{N-3}+a_{N-2}$$
From these series, it is clear that $A_{0} = a_{N-1}$ and that $A_{1} = a_{N}$
It is also clear that $a_{N-1}$ = $S_{N-1}-S_{N-2}$, and $a_{N} = S_{N}-S_{N-1}$.
Thus using these relations, and because we know that $\hat{T}_{N-2}$ is a converging geo series, we can use the equation $\frac{A_{0}}{1-r}$ to find the sum of $\hat{T}_{N-2}$. Thus, plugging our known values in, we get:
$$\hat{T}_{N-2} = \frac{{S_{N-1}-S_{N-2}}}{1-\frac{{S_{N}-S_{N-1}}}{S_{N-1}-S_{N-2}}}$$