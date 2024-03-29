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
To use the shell method, we need to integrate across x from 0 -> a, and create shells using the formula, $2\pi rh$:
Using the relationship from earlier, $z = -\frac{h}{a}r+h$, we can sub $z$ into $h$:
thus, the formula for the area of the shell is:
$$A=2\pi r\left( h-\frac{h}{a}r \right)$$
Thus, we take the integral of this from 0 -> a to get volume
$$V = 2\pi h \int_{0}^{a} r-\frac{r^2}{a} \, dr $$
$$= 2\pi h\begin{bmatrix}
\frac{r^2}{2}-\frac{r^3}{3a}
\end{bmatrix}_{0}^a$$
$$V = \frac{2\pi ha^2}{6}$$
$$= \frac{\pi ha^2}{3}$$
Thus, we get the same volume as part b.




d.
$$h = 1, r = a, b = 2r = 2a$$
$$A(0) = \frac{1}{2}bh = \frac{1}{2}*1*2a = a$$
e. To begin, we need to first find out the shape of the cross section, which is a hyperbola. To get the area as a definite integral, we need to integrate the hyperbola from 0 to the width of the cone at a certain $x_{0}$. To do that, we need to first get the width of the cone as a function of $x$: $$r(x) = \sqrt{ a^2-x^2 }$$ The height can be found from similar triangles using the known values at $x_{0}$ of $h = 1$, and $r = a$ $$\frac{h(x)}{r(x)} = \frac{1}{a}$$ $$h(x) = \frac{\sqrt{ a^2-x^2 }}{a}$$ Instead of using a negative slope and having to shift the line up by h, we can just use the positive line that crosses the origin, as it would give us the same area under the curve. $$m = \frac{h(x)}{r(x)}$$ $$y = mx$$ $$y = \frac{1}{a}x$$ Now that we have the equation of the line that gives us half of the triangle, we can integrate the function from 0 to the width of the smaller triangle, and multiply it by 2 to get the full area of the triangle: $$A(x_{0}) = 2\int_{0}^{\sqrt{ a^2-x_{0}^2 }} \frac{1}{a}t \, dt $$

### e.

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
$$\lim_{ x \to 0 } \sqrt{ a^2-x^2 }+\frac{x^2}{a}\ln\left( \frac{x}{a+\sqrt{ a^2-x^2 }} \right)$$
$$= a+ \lim_{ x \to 0 } \frac{x^2}{a}\ln\left( \frac{x}{2a} \right)$$
As $x$ approaches 0, $\ln\left( \frac{x}{2a} \right)$ approaches $-\infty$.
We can now manipulate this into a fraction:
$$\lim_{ x \to 0 } \frac{x^2}{a}\ln\left( \frac{x}{2a} \right)=\lim_{ x \to 0 } \frac{{\ln{ \left( \frac{x}{2a} \right)}}}{\frac{a}{x^2}}$$
Now, as we have the indeterminate form of $\frac{\infty}{\infty}$, we can use l'hospital's rule:
$$\lim_{ x \to 0 } \frac{\ln\left( \frac{x}{2a} \right)}{\frac{a}{x^2}} = \lim_{ x \to 0 } \frac{\frac{1}{x}}{\frac{-2a}{x^3}}$$
$$= \lim_{ x \to 0 } \frac{x^2}{-2a} = 0$$
Thus, we are left with just the first term, which was just $a$. Thus, we can see that as the limit of $A(x)$ approaches the value at 0, we can say that the function $A$ is continuous at 0.

### h.
For this part, we can prove that $F(x)$ is an anti-derivative of $A(x)$ by taking its derivative with respect to $x$, and comparing it to $A(x)$, $\sqrt{ a^2-x^2 }+\frac{x^2}{a}\ln\left( \frac{x}{a+\sqrt{ a^2-x^2 }} \right)$ 

$$F(x) 
= \frac{a^2}3\sin^{-1}\!({\frac xa})
   + \frac{2x}{3}\sqrt{a^2-x^2}
   + \frac{x^3}{3a}\log\mid{x}\mid
   - \frac{x^3}{3a}\log\mid{a+\sqrt{a^2-x^2}}\mid$$
   $$F'(x) = \frac{a}{3\sqrt{ 1-\frac{x}{a}^2 }} +\frac{2\sqrt{ a^2-x^2 }}{3}+\frac{\frac{2x}{3}*1}{2\sqrt{ a^2-x^2 }}*(-2x) + \frac{x^2}{a}\ln |x|+\frac{x^2}{3a}-\left( \frac{x^2}{a}\ln \mid a+\sqrt{ a^2-x^2 } \mid  \right)-\frac{x^3}{3a}* \frac{-2x* \frac{1}{2}(a^2-x^2)^{-1/2}}{a+\sqrt{ a^2-x^2 }}$$
   $$= \frac{a}{3\sqrt{ 1-\left( \frac{x}{a} \right)^2 }} + \frac{2\sqrt{ a^2-x^2 }}{3}+\frac{-2x^2}{3\sqrt{ a^2-x^2 }}+\frac{x^2}{a}(\ln \mid x \mid -\ln \mid a+\sqrt{ a^2-x^2 } \mid )+\frac{x^2}{3a}+\left(\frac{x^4}{(3a\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 }))} \right)$$
   Dealing with just the term, $\frac{x^2}{a}(\ln|x| - \ln \mid a+\sqrt{ a^2-x^2 } \mid)$, we can simplify it:
   $$\frac{x^2}{a}\left( \ln | \frac{x}{a+\sqrt{ a^2-x^2 }} | \right)$$
We can also multiply this term by $\frac{3}{3}$ to combine it with the term, $\frac{x^2}{3a}$:
$$\frac{{3x^2\left( \ln \mid \frac{x}{a+\sqrt{ a^2-x^2 }} \mid  \right)+x^2}}{3a}$$
$$=\frac{x^2}{3a}\left( 3\ln \mid \frac{x}{a+\sqrt{ a^2-x^2 }} \mid  +1\right)$$
$$\frac{x^2}{a}\ln \mid \frac{x}{a+\sqrt{ a^2-x^2 }} \mid +\frac{x^2}{3a}$$
Adding this back into the original, we get:
$$= \frac{a}{3\sqrt{ 1-\left( \frac{x}{a} \right)^2 }} + \frac{2\sqrt{ a^2-x^2 }}{3}+\frac{-2x^2}{3\sqrt{ a^2-x^2 }}+
\frac{x^2}{a}\ln \mid \frac{x}{a+\sqrt{ a^2-x^2 }} \mid +\frac{x^2}{3a}
+\left(\frac{x^4}{(3a\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 }))} \right)$$
Focusing on the 2 terms, 
$$\frac{2\sqrt{ a^2-x^2 }}{3}+\frac{-2x^2}{3\sqrt{ a^2-x^2 }}$$
we can use a common denominator to combine them:
$$\frac{{2\sqrt{ a^2-x^2 }*\sqrt{ a^2-x^2 }-2x^2}}{3\sqrt{ a^2-x^2 }}$$
$$= \frac{2(a^2-2x^2)}{3\sqrt{ a^2-x^2 }}$$
combining this with the term, $\frac{x^2}{3a}$,
$$\frac{2(a^2-2x^2)}{3\sqrt{ a^2-x^2 }}+\frac{x^2}{3a}$$
$$= \frac{2a(a^2-2x^2)+x^2(\sqrt{ a^2-x^2 })}{3a\sqrt{ a^2-x^2 }}$$
$$= \frac{{2a^3-4ax^2+x^2\sqrt{ a^2-x^2 }}}{3a\sqrt{ a^2-x^2 }}$$
Plugging everything back in, our equation looks like this:

$$F'(x)=\frac{a}{3\sqrt{ 1-\frac{x^2}{a^2} }}+ \frac{{2a^3-4ax^2+x^2\sqrt{ a^2-x^2 }}}{3a\sqrt{ a^2-x^2 }}+\left(\frac{x^4}{(3a\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 }))} \right)+\frac{x^2}{a}\ln ( \frac{x}{a+\sqrt{ a^2-x^2 }} )$$
$$= \frac{a^3}{3a\sqrt{ a^2-x^2 }}+\frac{{2a^3-4ax^2+x^2\sqrt{ a^2-x^2 }}}{3a\sqrt{ a^2-x^2 }}+\frac{x^4}{3a\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 })}+
\frac{x^2}{a}\ln ( \frac{x}{a+\sqrt{ a^2-x^2 }} )	
$$
The original equation, $A(x)= \sqrt{ a^2-x^2 }+\frac{x^2}{a}\ln\left( \frac{x}{a+\sqrt{ a^2-x^2 }} \right)$, matches the last term in $F'(x)$, so I will omit the last term to make it a little simpler for now:
$$\frac{{(3a^3-4ax^2+x^2\sqrt{ a^2-x^2 })(a+\sqrt{ a^2-x^2 })+x^4}}{3a\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 })}$$
Because the remaining terms share the same denominator, we can also omit it for now, and add it back later:
$${3a^4-4a^2x^2+ax^2\sqrt{ a^2-x^2 }+3a^3\sqrt{ a^2-x^2 }-4ax^2\sqrt{ a^2-x^2 }+x^2a^2-x^4+x^4}$$
$$= 3a^4-3a^2x^2+(3a^3-3ax^2)(\sqrt{ a^2-x^2 })$$
Re-introducing the denominator,
$$\frac{{3a^4-3a^2x^2+(3a^3-3ax^2)(\sqrt{ a^2-x^2 })}}{3a\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 })}$$
$$= \frac{{a^3-ax^2+(a^2-x^2)(\sqrt{ a^2-x^2 })}}{\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 })}$$
$$= \frac{{a(a^2-x^2)+(a^2-x^2)(\sqrt{ a^2-x^2 })}}{\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 })}$$
$$= \frac{{(a+\sqrt{ a^2-x^2 })(a^2-x^2)}}{\sqrt{ a^2-x^2 }(a+\sqrt{ a^2-x^2 })}$$
$$=\frac{{a^2-x^2}}{\sqrt{ a^2-x^2 }}$$
Adding back the term I originally omitted, and simplifying the equation one last time, we get:
$$F'(x) = \sqrt{ a^2-x^2 } + \frac{x^2}{a}\ln ( \frac{x}{a+\sqrt{ a^2-x^2 }})$$
Thus, as $A(x) = \sqrt{ a^2-x^2 }+\frac{x^2}{a}\ln\left( \frac{x}{a+\sqrt{ a^2-x^2 }} \right)$, we can see that $F'(x)$ indeed equals to $A(x)$.


### i.
Using the function,
$$A(x) = \sqrt{ a^2-x^2 }+\frac{x^2}{a}\ln\left( \frac{x}{a+\sqrt{ a^2-x^2 }} \right)$$
, we now know that it's anti-derivative is indeed $F(x)$. Thus, to find the volume of the cone, we can evaluate $F(x)|_{-a}^a$ to get the volume:
$$F(x) 
= \frac{a^2}3\sin^{-1}\!({\frac xa})
   + \frac{2x}{3}\sqrt{a^2-x^2}
   + \frac{x^3}{3a}\log\mid{x}\mid
   - \frac{x^3}{3a}\log\mid{a+\sqrt{a^2-x^2}}\mid$$
$$F(a)-F(-a)=\frac{a^2}3\sin^{-1}\!(1)
   + \frac{2a}{3}\sqrt{a^2-a^2}
   + \frac{a^3}{3a}\log\mid{a}\mid
   - \frac{a^3}{3a}\log\mid{a+\sqrt{a^2-a^2}}\mid - (
\frac{a^2}3\sin^{-1}\!(-1)
   + \frac{2(-a)}{3}\sqrt{a^2-(-a)^2}
   + \frac{(-a)^3}{3a}\log\mid{-a}\mid
   - \frac{(-a)^3}{3a}\log\mid{a+\sqrt{a^2-(-a)^2}}\mid)
$$
$$= \frac{a^2}{3} * \frac{\pi}{2}+\frac{a^2}{3}\ln|a|-\frac{a^2}{3}\ln|a|-\left( \frac{a^2}{3}\left( -\frac{\pi}{2} \right)- \frac{a^2}{3}\ln|-a|+\frac{a^2}{3} \ln|a| \right)$$
$$= \frac{a^2\pi}{6}+ \frac{a^2\pi}{6}+\frac{a^2}{3}\ln(a)-\frac{a^2\ln(a)}{3}$$
$$=\frac{a^2\pi}{3}$$
Thus, we can see that the volume of the cone is $\frac{a^2\pi}{3}$