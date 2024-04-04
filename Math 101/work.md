Knowing that $f(t) = 0$ for every other integer interval, we can write $F(s)$ as an infinite series of integrals:
$$F(s) = \int_{0}^{1} e^{-st} \, dt  + \int_{2}^{3} e^{-st} \, dt + \int_{4}^{5} e^{-st} \, dt +\dots + \int_{2n}^{2n+1} e^{-st} \, dt $$
Evaluating the anti-derivative for $\int e^{-st} \, dt$, we get:
$$\int e^{-st} \, dt  = -\frac{1}{se^{st}}+C$$
And now, plugging this into $F(s)$,
$$F(s) = -\frac{1}{se^s}+\frac{1}{s}-\frac{1}{se^{3s}}+\frac{1}{se^{2s}}-\frac{1}{se^{5s}}+\frac{1}{se^{4s}}+\dots-\frac{1}{se^{(2n+1)s}}+\frac{1}{se^{2ns}}$$
Rearranging these to make them go in order of the power of e, we get:
$$F(s) = \frac{1}{s} - \frac{1}{se^s}+\frac{1}{se^{2s}} - \frac{1}{se^{3s}} + \frac{1}{se^{4s}} + \dots + \frac{1}{se^{2ns}} - \frac{1}{se^{s(2n+1)}}$$
From this, we can see that $F(s)$ is a geometric series, with the first term being $\frac{1}{s}$, and the factor being $-\frac{1}{e^s}$
Thus, using the formula for a geometric series, $\frac{a}{1-r}$, where $a$ is the first term, and $r$ is the factor, we can see that $F(s) = \frac{\frac{1}{s}}{1+\frac{1}{e^s}}$ 
Thus,
$$F(s) = \frac{\frac{1}{s}}{\frac{{e^s+1}}{e^s}}=\frac{e^s}{s(e^s+1)}$$
Simplifying this, we get
$$F(s) = \frac{1}{s(1+e^{-s})}$$
, which is exactly what we are looking for.