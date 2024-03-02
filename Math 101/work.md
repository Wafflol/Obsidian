a.
$$\frac{a}{h} = \frac{r}{h-z}$$
$$ha-za=rh$$
$$ha-rh=za$$
$$z = \frac{{ha-rh}}{a}$$
$$f(r) = z = h-\frac{rh}{a}$$

b.
$$\frac{{ha-za}}{h}=r$$$$a-\frac{za}{h} = r$$
$$V = \pi \int_{0}^{h} (a-\frac{za}{h})^2 \, dz $$
$$=\pi \int_{0}^{h} a^2-\frac{2za^2}{h}+\frac{z^2a^2}{h^2} \, dz $$
$$ = \pi \begin{bmatrix}
a^2z-\frac{z^2a^2}{h} + z ^3 \frac{a^2}{3h^2}
\end{bmatrix}_{0}^h$$
$$=\pi\left( \frac{h^3a^2}{3h^2} \right)$$
$$ = \frac{\pi ha^2}{3}$$
c.
$$V = \pi \int_{0}^{h} \left( a^2-\frac{2za^2}{h}+\frac{z^2a^2}{h^2} \right)z \, dx $$
$$= \pi \begin{bmatrix}
\frac{a^2z^2}{2}-\frac{2z^3a^2}{3h}+\frac{z^4a^2}{4h^2}
\end{bmatrix}_{0}^h$$
$$ = \pi\left( \frac{a^2h^2}{2}-\frac{2a^2h^2}{3}+\frac{h^4a^2}{4h^2} \right)$$
$$=-\frac{\pi a^2h^2}{6}+\frac{\pi a^2h^2}{4}$$
$$ = \frac{\pi a^2h^3}{12}$$
d.
$$h = 1, r = a, b = 2r = 2a$$
$$A(0) = \frac{1}{2}bh = \frac{1}{2}*1*2a = a$$
e. To begin, we need to first find out the shape of the cross section, which is a hyperbola. To get the area as a definite integral, we need to integrate the hyperbola from 0 to the width of the cone at a certain $x_{0}$. To do that, we need to first get the width of the cone as a function of $x$: $$r(x) = \sqrt{ a^2-x^2 }$$ The height can be found from similar triangles using the known values at $x_{0}$ of $h = 1$, and $r = a$ $$\frac{h(x)}{r(x)} = \frac{1}{a}$$ $$h(x) = \frac{\sqrt{ a^2-x^2 }}{a}$$ Instead of using a negative slope and having to shift the line up by h, we can just use the positive line that crosses the origin, as it would give us the same area under the curve. $$m = \frac{h(x)}{r(x)}$$ $$y = mx$$ $$y = \frac{1}{a}x$$ Now that we have the equation of the line that gives us half of the triangle, we can integrate the function from 0 to the width of the smaller triangle, and multiply it by 2 to get the full area of the triangle: $$A(x_{0}) = 2\int_{0}^{\sqrt{ a^2-x_{0}^2 }} \frac{1}{a}t \, dt $$

e rewrite.

To start off, we know that a vertical slice of a cone is a hyperbola.
We can first find the width of half the base at each slice:
$$r(x) = \sqrt{ a^2-x^2 }$$
Then, we can use an altered version of the hyperbola equation to get the shape of the slice at each $x_{0}$:
$$z = 1-\frac{1}{a}\sqrt{ x_{0}^2+y^2 }$$
where $r$ is the $r(x)$ we found earlier.
Thus, our definite integral for any $x_{0}$ for $0< x_{0} < a$ is:
$$A(x_{0}) = 2\int_{0}^{\sqrt{ a^2-x_{0}^2 }} 1-\frac{1}{a}\sqrt{ x_{0}^2+y^2 } \, dy $$
f.
Now, we just have to evaluate the given integral:
starting with the second term, we have:
$$\frac{1}{a}\int_{0}^{\sqrt{ a^2-x_{0}^2 }} \sqrt{ x_{0}^2+y^2 } \, dy $$
leaving $\frac{1}{a}$ out for now, we can to trig sub here:
$$y = x_{0}tan \theta$$
$$dy = x_{0}\sec^2\theta d\theta$$
$$\int_{\theta(0)}^{\theta(\sqrt{ a^2-x_{0}^2 })} {\sqrt{ x_{0}^2+{x_{0}^2\tan^2\theta} }*\sec^2\theta*x_{0}} \, d\theta $$
$$ = x_{0}^2\int_{\theta(0)}^{\theta(\sqrt{ a^2-x_{0}^2 })} \sec^3\theta \, d\theta $$
Using the famous anti-derivative for $\sec^3\theta$, we get:
$$x_{0}^2\int_{\theta(0)}^{\theta(\sqrt{ a^2-x_{0}^2 })} \sec^3\theta \, d\theta $$
$$=x_{0}^2\begin{bmatrix}
\frac12\sec\theta\tan\theta + \frac12\log|{\sec\theta+\tan\theta}|
\end{bmatrix}_{\theta(0)}^{\theta(\sqrt{ a^2-x_{0}^2 })}$$
subbing y back and using the original bounds,
$$= x_{0}^2\left( \frac{1}{2}\left( \frac{\sqrt{ x_{0}^2+a^2-x_{0}^2 }}{x_{0}} \frac{\sqrt{ a^2-x_{0}^2 }}{x_{0}}+\ln\left( \frac{\sqrt{ a^2 }}{x_{0}}+\frac{\sqrt{ a^2-x_{0}^2 }}{x_{0}} \right) \right) \right)$$
$$=\frac{x_{0}^2}{2}*\left( \frac{a\sqrt{ a^2-x^2 }}{x_{0}^2} +\ln\left( \frac{{a+\sqrt{ a^2-x_{0}^2 }}}{x_{0}} \right)\right)$$
Multiplying $\frac{1}{a}$ back, we get:
$$=\frac{x_{0}^2}{2a}*\left( \frac{a\sqrt{ a^2-x^2 }}{x_{0}^2} +\ln\left( \frac{{a+\sqrt{ a^2-x_{0}^2 }}}{x_{0}} \right)\right)$$
Now, integrating the first term:
$$\int_{0}^{\sqrt{ a^2-x_{0}^2 }} 1 \, dy $$
$$= \sqrt{ a^2-x^2 }$$
Putting them together, and adding the multiple of two back in, we get:

$$A(x_{0}) = 2\sqrt{ a^2- x_{0}^2 } - \frac{x_{0}^2}{a}*\left( \frac{a\sqrt{ a^2-x^2 }}{x_{0}^2} +\ln\left( \frac{{a+\sqrt{ a^2-x_{0}^2 }}}{x_{0}} \right)\right)$$
$$= \sqrt{ a^2-x_{0}^2 }+\frac{x_{0}^2}{a}\ln\left( \frac{x_{0}}{a+\sqrt{ a^2-x_{0}^2 }} \right)$$
Changing $x_{0}$ to $x$,
$$A = A(x) = \sqrt{ a^2-x^2 }+\frac{x^2}{a}\ln\left( \frac{x}{a+\sqrt{ a^2-x^2 }} \right)$$
### g.
To show that A is continuous at 0, we can take the limit of A(x) as it approaches 0 from the positive side, and show that it is equal to the value at 0, which we found in part d, which is A = $a$.
$$\lim_{ n \to \infty } $$