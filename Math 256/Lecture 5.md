### Second Order Linear ODE
$$Ly = y'' + p(x)y'+ q(x)y + g(x)$$
$$=0 \Rightarrow \text{homogeneous}$$
$$\neq 0 \Rightarrow \text{inhomogeneous}$$

Eg.
$$p=0, q=0 \Rightarrow y''=g(x)$$
$$y(x)  = \int \int g(s) \, ds  \, dx +Cx+D$$
- 2 arbitraty const
- 2 solutions to homog eq {x, 1}

#### Initial Value Problems (IVP)
$$y(x_{0}) = y_{0}, y'(x_{0}) = v_{0}$$
#### Boundary Value Problems (BVP)
$$y(x_{0}) = y_{0}, y(x_{1})=y_{1}$$
2 values

---

EG:
$$Ly = y'' + y' - 6y = 0$$
$$y(0) = 0, y'(0) =5$$
Guess: $y = e^{rx}$
$$y' = r e^{rx}$$
$$y''=r^2e^{rx}$$
$$Le^{rx} = [r^2+r-6]e^{rx}$$
$$e^{rx} \neq 0 \Rightarrow r^2+r-6=0$$
$$r=-3, 2$$
$$y(x)=Ae^{-3x}+Be^{2x}$$
$$y'(x)=-3Ae^{-3x}+2Be^{2x}$$
$$0=A+B=y(0) \Rightarrow A=-B$$
$$5=-3A+2B=y'(0)$$
$$5 = 5B, B=1, A=-1$$
$$A=-1$$
$$y(x) = -e^{-3x} + e^{2x}$$
---
EG:
$$Ly=x^2y''+2xy'-2y=0$$
$$y(1)=3, y'(1)=0$$
Find y: 
$$xy'=ry$$
$$\int \frac{1}{y} \, dy =r \int \frac{1}{x} \, dx +C$$
$$y=Ax^r$$
$$A=e^c$$
Guess:
$$y=x^r$$
$$y'=rx^{r-1}$$
$$y''=r(r-1)x^{r-2)}$$
$$L(x^r)=x^2\{r(r-1)x^{r-2}\}+2x\{rx^{r-1}\}-2x^r=0$$
Therefore: 
$$[r^2+r-2]x^r=0$$
$$ \Rightarrow r^2+r-2=0$$
$$r_{1}=-2, r_{2}=1$$
$$y(x)=Ax+Bx^{-2}$$
$$y'(x)=A-2Bx^{-3}$$
$$B=1, A=2$$
$$y(x)=2x+x^{-2}$$