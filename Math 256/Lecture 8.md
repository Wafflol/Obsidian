### Homogeneous 2nd Order Linear ODE
#### Constant Coefficient Case
$$Ly=ay''+by'+cy=g(x)$$
Homogeneous eq:
$$g(x)=0, y=e^{rx}$$
$$\Rightarrow ar^2+br+c=0$$
$$r=\frac{-b\pm \sqrt{ b^2-4ac }}{2a}$$
$$\Delta = b^2-4ac$$
$$\Delta>0, r_{1}, r_{2}, y_{H}=c_{1}e^{r_{1}x}+c_{2}e^{r_{2}x}$$
$$\Delta = 0, r_{1} = -\frac{b}{2a}, y_{H}=c_{1}e^{r_{1}x}+c_{2}xe^{r_{1}x}$$
$$\Delta < 0, r= \alpha\pm i\beta, y_{H}(x)=e^{\alpha x}(A\cos\beta x+B\sin(\beta x))$$
General solution of form
$$y(x) = y_{H}(x) + y_{P}(x)$$
### Using Method of Undetermined Coeff To Find $y_{p}(x)$
1. guess $y_{P}(x)$ from the family of all possible derivatives of $g(x)$
2. plug into $1.$ $Ly_{p}=g(x)$. Collect like functions/powers on left side and match to RHS

| $y(x)$                 | Guess $y_{P}$                    |
| ---------------------- | -------------------------------- |
| $e^{ax}$               | $Ae^{ax}$                        |
| $x^n$                  | $a_{n}x^n+a_{n-1}x^{n-1}+\dots+$ |
| $\sin ax$ or $\cos ax$ | $A\cos ax+B\sin ax$              |
EG:
$$Ly=ay''+by'+cy=e^{\omega x}$$
$$y_{p}=Ae^{\omega x}, y_{p}'=A \omega e^{\omega x}, y_{p}''=A\omega^2e^{ \omega x }$$
$$Ly_{p}=A(a\omega^2+b\omega+c)e^{\omega x}=e^{\omega x}$$
$$A=\frac{1}{a\omega+b\omega+c}$$
---

Eg