### Linear Dependence of FCNS
Let $f$ and $g$ be 2 functions defined on an interval $I$. Then $f$ and $g$ are linearly dependent if there exist $k_{1}+k_{2}$ (Not both 0) such that $k_{1}f+k_{2}g=0$

#### Last Class
If $y_{2}(x)=Cy_{1}(x)$ then
$$W(x) = \begin{vmatrix}
y_{1} & y_{2} \\
y_{1}' & y_{2}'
\end{vmatrix}=0$$
If $W(x)=0$ on an interval $I$ then
$$y_{2}(x)=Cy_{1}(x)$$

#### Theorem
If $y_{1}$ and $y_{2}$ are solutions to the homogeneous eq,
$$Ly=y'' + py'+qy=0$$
Then if $W(x) = y_{1}y_{2}'-y_{1}'y_{2}\neq 0$ for some $x_{0} \in I$, then $W(x) \neq 0$ for all $x \in I$
$$W'=y_{1}y_{2}''-y_{1}''y_{2}$$
$$=-p(x)W(x)$$
$$\int \frac{1}{W} \, dW=-\int p(x) \, dx +c$$
$$W(x) = Ae^{-\int p(x) \, dx }$$
$$W(x_{0})=Ae^{\int^{x_{0}} p(s)  \, ds }$$
$$W(x)=W(x_{0})e^{\int_{x}^{x_{0}} p(s) \, ds } $$
$$W(x_{0})\neq 0 \Rightarrow W(x) \neq 0 \forall x \in I$$
___
### Fundamental Set of Solutions
Let $y_{1}(x)$ and $y_{2}(x)$ be linearly independent solutions of the homogeneous equation
$$Ly=0$$
Then $\{y_{1}(x), y_{2}(x)\}$ form a fundamental set of solutions and the general solution to $Ly=0$ is of the form $y_{H}=C_{1}y_{1}+C_{2}y_{2}$

---
### Constant Coefficient 2nd Order Linear ODE
$$Ly = ay''+by'+Cy=0$$
$$L := a \frac{d^2}{dx^2}+ b \frac{d}{dx} + C= a D^2 + bD+C$$
$$y=e^{rx}$$
$$y'=r e^{rx}$$
$$y'' = r^2 e^{rx}$$
$$Le^{rx} = [ar^2+br+c]e^{rx}=0$$
Characteristic Eq:
$$e^{rx}\neq 0 \Rightarrow ar^2+br+c=0$$
$$r= \frac{-b\pm \sqrt{ b^2-4ac }}{2a}$$
Discriminant:
$$\Delta = b^2-4ac$$
##### Case 1:
$$\Delta=b^2-4ac>0$$
2 real roots, $r_{1}, r_{2}$
$$y_{H}(x)=C_{1}e^{r_{1}x}+C_{2}e^{r_{2}x}$$
Are $y_{1} = e^{r_{1}x}$ and $y_{2}=e^{r_{2}x}$ linearly independent?
$$W(x) = \begin{vmatrix}
e^{r_{1}x} & e^{r_{2}x} \\
r_{1}e^{r_{1}x}  &  r_{2}e^{r_{2}x}
\end{vmatrix} = r_{2}e^({r_{1}+r_{2})x}-r_{1}e^{(r_{1}+r_{2})x}$$
$$=(r_{2}-r_{1})e^{(r_{1}+r_{2})x}$$
##### Case 2:
$$\Delta = b^2-4ac=0$$
$$r_{1}=-\frac{b}{2a}$$
$$Ly = (aD^2+bD+c)y=0$$
$$=a\left[ \left( D+\frac{b}{2a} \right)^2-\frac{b^2}{4a^2}+\frac{4ac}{4a^2} \right]$$
$$=a\left[ \left( D+\frac{b}{2a^2} \right) \right]$$
$$L=a\left( D+\frac{b}{2a} \right)^2$$
$$Ly=a(D-r_{1})^2y=0$$
$$(D-r_{1})(D-r_{1})y=0$$
Let
$$(D-r_{1})y=\omega$$
$$(D-r_{1})\omega=0$$
$$\frac{d\omega}{dx}-r_{1}\omega=0$$
$$\frac{d}{dx}[e^{-r_{1}x}\omega]=0$$
$$e^{-r_{1}x}\omega=C_{1}$$
$$\omega=C_{1}e^{r_{1}x}$$
Solve $(D-r_{1})y=\omega=C_{1}e^{r_{1}x}$
$$\frac{dy}{dx}-r_{1}y=c_{1}e^{r_{1}x}$$
$$e^{-r_{1}x}y'-r_{1}e^{-r_{1}x}y=C_{1}e^{-r_{1}x}e^{r_{1}x}$$
$$\frac{d}{dx}[e^{-r_{1}x}y]=C_{1}$$
$$e^{-r_{1}x}y=C_{1}x+C_{2}$$
$$y(x)=C_{1}xe^{r_{1}x}+C_{2}e^{r_{1}x}$$
$$y_{H}(x) = C_{1}e^{r_{1}x}+C_{2}xe^{r_{1}x}$$
Check: $y_{1}$ and $y_{2}$ are [[Linear indenpendence | Linearly Independent]]

---

##### Case 3
$$r = - \frac{b}{2a}\pm\frac{\sqrt{ \Delta }}{2a}$$
$$r = - \frac{b}{2a}\pm\frac{\sqrt{- (- \Delta) }}{2a}$$
$$=-\frac{b}{2a}\pm i \frac{\sqrt{ -\Delta }}{2a}$$
$$=\alpha\pm i\beta$$
$$\alpha=-\frac{b}{2a}$$
$$\beta=\frac{\sqrt{ -\Delta }}{2a}$$
$$r=\alpha\pm i\beta$$
Complex Conjugate roots
$$y(x)=e^{(\alpha\pm i\beta )x}$$
$$y_{1}(x)=e^{(\alpha+ i\beta )x}$$
We want solutions that are real fcns
$$\frac{{y_{1}+y_{2}}}{2}=e^{\alpha x}\cos(\beta x)$$
$$\frac{{y_{1}-y_{2}}}{2}=e^{\alpha x}\sin(\beta x)$2$