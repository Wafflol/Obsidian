### Linear Variable Coeff 2nd Order ODEs
$$Ly = y'' + p(x)y' + q(x)y = g(x)$$
If $y_{1}(x) \& y_{2}(x)$ are linearly independent solutions to the homogeneous eq $Ly_{H}(x) = 0$, then the general solution is of the form
$$y_{H}(x)=c_{1}y_{1}(x)+c_{2}y_{2}(x)$$
If $y_{p}(x)$ is any particular solution, $Ly_{p}=g(x)$, then the general solution
$$y(x)=y_{H}(x)+y_{p}(x)$$
---
#### Euler EQ
$$Ly=ax^2y''+bxy'+cy=g(x)$$
EG:
$$a=0, b=1, c=-r, g=0$$
$$x \frac{dy}{dx} = ry$$
$$\int \frac{1}{y} \, dy=\int \frac{r}{x} \, dx +c $$
$$e^{\ln y}=e^{\ln x^r+c}$$
$$y=Ax^r$$
Back to:
$$Ly=ax^2y''+bxy'+cy=0$$
Guess $y = x^r, y'=rx^{r-1}, y''=r(r-1)x^{r-2}$
$$Lx^r=ax^2r(r-1)x^{r-2}+bxrx^{r-1}+cx^r=0$$
$$(ar(r-1)+br+c)x^r=0 \forall x$$
$$\Rightarrow ax^2+(b-a)r+c=0$$
$$r_{1,2} = \frac{-(b-a)\pm \sqrt{ (b-a)^2-4ac}}{2a}$$
$$\Delta = (b-a)^2-4ac, \text{ discriminant}$$
##### $$1.) \Delta > 0 \Rightarrow \text{2 distinct real roots } r_{1} \& r_{2}$$
$$y(x) = c_{1}x^{r_{1}} + c_{2}x^{r_{2}}$$
EG:
$$Ly = x^2y''+xy'-9y=0$$
$$y=x^r \Rightarrow (r(r-1)+r-9)x^r=0$$
$$r^2-9=0 = \pm {3}$$
$$y(x) = c_{1}x^3+c_{2}x^{-3}$$
#### $$2.) \Delta < 0 \Rightarrow \text{ complex conjugate pair } r_{1,2}$$
$$r_{1,2}=-\frac{b-a}{2a} \pm \frac{\sqrt{ 4ac-(b-a)^2 }}{2a}=\alpha\pm i\beta$$
$$y(x)=x^{\alpha\pm i\beta}$$
$$=x^{\alpha}x^{\pm i\beta}$$
$$=x^\alpha e^{i\beta \ln x}$$
$$=x^\alpha(\cos(\beta \ln x)\pm i\sin\beta \ln x)$$

####  $$3.)\Delta = 0, r_{1} \text{ is a double root}$$
$$r_{1} = -\frac{b-a}{2a}$$
$$y_{1}(x)=c_{1}x^{r_{1}} \text{ is a solution }$$
How do we get a 2nd?
$$Lx^r=(ar^2+(b-a)r+c)x^r=0$$
$$=a\left( r^2+\left( \frac{b-a}{2a} \right)^2-\frac{\sqrt{ (b-a)^2-4ac }}{4a^2} \right)$$
$$=a(r-r_{1})^2=0$$
$$a(r-(r_{1}+\epsilon))(r-(r_{1}-\epsilon))=0$$
$$y(x)=c_{1}x^{r_{1}+\epsilon}+c_{2}x^{r_{1}-\epsilon}$$
choose $c_{1}=\frac{1}{2\epsilon}, c_{2}=-\frac{1}{2\epsilon}$
$$y_{2}(x)=\lim_{ \epsilon \to 0 } \frac{x^{r_{1}+\epsilon}-x^{r_{1}-\epsilon}}{2\epsilon}= \frac{\partial}{\partial r} x^2|_{r=r_{1}}$$
$$y_{2}(x)=\frac{\partial}{\partial r}e^{r\ln x}|_{r=r_{1}}$$
$$=e^{r\ln x}\ln x|_{r=r_{1}}$$
$$y_{2}=x^{r_{1}}\ln x$$
$$y_{H}(x)=c_{1}x^{r_{1}}+c_{2}x^{r_{1}}\ln x$$
Remember for $ay''+by'+cy=0$
$$y=e^{rx}, ar^2+br+c=0$$
$$r_{1,2}=\frac{-b\pm \sqrt{ b^2-4ac }}{2a}$$
$$\Delta = b^2-4ac=0$$
$$y_{1}=e^{r_{1}x}, r_{1}=-\frac{b}{2a}$$
$$\frac{\partial}{\partial r}e^{rx}|_{r_{1}}=xe^{r_{1}x}$$
$$y(x)=c_{1}e^{r_{1}x}+c_{2}xe^{r_{1}x}$$
#### Method of Reduction of Order
$$Ly = y''+p(x)y'+q(x)y=g(x)$$
And assume $y_{1}(x)$ is a solution of the homogeneous eq
I.e. $Ly_{1}=y_{1}''+py_{1}'+qy_{1}=0$

Let $y_{2}(x)=u(x)y_{1}(x)$
$$y_{2}'(x)=uy_{1}'+u'y_{1}$$
$$y_{2}''(x)=uy_{1}''+2u'y_{1}'$$
$$Ly_{2}=u\{y_{1}''+py_{1}'+qy_{1}\}+u''y_{1}+(2y_{1}'+py_{1})u'$$
$$\{\dots\} = 0, \text{ as } Ly_{1}=0$$
$$u''+\left( \frac{2y_{1}'}{y_{1}}+p(x) \right)u'=\frac{g(x)}{y_{1}(x)}$$
Linear 1st order eq for $u'$
$$F(x)=e^{\int 2y_{1}'/y \, dx + \int px \, dx }   $$
$$F(x) = y_{1}^2e^{\int p(x) \, dx }$$
$$(F(x)u')'=F(x)u''+\left( \frac{2y_{1}'}{y_{1}}+p(x))F(x)u' \right) = \frac{F(x)g(x)}{y_{1}(x)}$$
