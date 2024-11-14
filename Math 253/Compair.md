The distance to a point $(x, y)$ from the origin is given as:
$$D = \sqrt{ x^2+y^2 }$$
However, for the purpose of this problem, we can take the square root away to simplify, since it only scales the magnitude.

Thus, we get $D = x^2+y^2$
We want to find when this equation is a minimum, so we use the lagrange multiplier method:

$$\nabla D = \lambda \nabla V$$
where $V = x^2y-16$

$$\nabla D = (2x, 2y)$$
$$\nabla V = (2xy, x^2)$$
Thus,
$$2x=2 \lambda xy, 2y = \lambda x^2$$
Using the second equation, $\lambda = \frac{2y}{x^2}$

Subbing this in to the first, you get: 
$$x=\frac{2y^2}{x}$$
$$x^2 = 2y^2$$
$$x=2y$$
Since we know the curve is bounded so that $x^2y=16$, it follows that $\frac{x^3}{2}=16$
$$x^3=32$$
$$$$