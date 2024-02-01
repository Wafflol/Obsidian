Using the general formula for the moving average, we can get the following equation:
$$
\bar{C}_{101}=\int_{t-1}^{t} ax^2+bx+C \, dx = \alpha t^2+\beta t+\gamma
$$
We can take the anti-derivative, which gives us:
$$
=\begin{bmatrix}
\frac{ax^3}{3}+\frac{bx^2}{2}+cx
\end{bmatrix}_{t-1}^t
$$
From here, we can simplify, and we get an equation that takes on the form of $\alpha t^2+\beta t+\gamma$
$$
= \frac{3at^2-3at+a}{3}+\frac{2bt-b}{2}+C
$$
$$
=at^2+(b-a)t+\left( \frac{a}{3}-\frac{b}{2}+c \right) = \alpha t^2+\beta t+\gamma
$$

Plugging in the numbers given in the problem, we get the following:
$$
\bar{C}_{101} = at^2+(b-a)t+\left( \frac{a}{3}-\frac{b}{2}+c \right)=  0.12997t^2-50.125t+48631
$$
Thus,
$$
a = \alpha = 0.012997
$$
$$
b = \beta + a = -50.112
$$
$$
c = \gamma-\frac{a}{3}+\frac{b}{2}=48605
$$
