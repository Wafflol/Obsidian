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
Since we know the curve is bounded so that $x^2y=16$, it follows that:
$$2y^3=16$$
$$y^3 = 8$$
$$y = 2$$
$$x^2= 2(2)^2=8$$
$$x = \pm2\sqrt{ 2 }$$

Plugging the x and y values we found ($\pm$ doesn't matter since it's squared), we find that 
D = $\sqrt{ 4+8 } = \sqrt{ 12 } = 2\sqrt{ 3 }$
Thus, the min dist from the origin to the curve $x^2y=16$ is $2\sqrt{ 3 }$