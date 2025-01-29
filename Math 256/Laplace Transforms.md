Work for constant coeff linear ode initial value problems
$$Ly = ay'' + by' + cy = g(t)$$
Initial values, $y(0) = y_{0}, y'(0) = v_{0}$
Fantastic for forcing functions $g(t)$ that have jumps or are impulses
$$Ly(t)=g(t)$$
##### Definition
Let $f$ be a piece wise continuous function defined on $[0, \infty)$ and assume $\mid f(t) \mid  < ke^{bt}, b>0$, then the laplace transform is defined as
$$\mathcal{L}(f(t))(s) = F(s) = \int_{0}^{\infty} e^{-st} f(t) \, dt , s>0 $$
###### 1.
$$\begin{align}
\mathcal{L}(1) &= \int_{0}^{\infty} e^{-st} \, dt  \\
&= \frac{e^{-st}}{-s}|_{0}^\infty=\frac{1}{s}  \\
\end{align}$$
$$\mathcal{L}(1) = \frac{1}{s}$$
###### 2.
$$\mathcal{L}(e^{at}) = \int_{0}^{\infty} e^{-st}e^{-at} \, dt$$
$$ = \int_{0}^{\infty} e^{-s+a}t \, dt $$
$$\mathcal{L}(e^{-at}) = \frac{1}{s+a}, s>a$$
###### 3.
Laplace transform is a linear operation
$$\mathcal{L}(\alpha f(t)+\beta g(t)) = \int_{0}^{\infty} e^{-st}(\alpha f(t)+\beta g(t)) \, dx $$

$$=\alpha F(s)+\beta G(s)$$
EG:
$$\mathcal{L}(c 1) = c\mathcal{L}(1)=\frac{c}{s}$$
###### 4.
Laplace transform of the derivatives of $f(t)$
$$
\begin{align}
\mathcal{L} (f'(t)) &= \int_{0}^{\infty} e^{-st}f'(t) \, dt  \\
\text{(ibp)} &= -f(0)+sF(s)
\end{align}$$
$$\mathcal{L}(f'(t)) = sF(s)-f(0)$$
---
$$\mathcal{L}(f''(t))=\int_{0}^{\infty} e^{-st}f''(t) \, dt $$
$$=e^{-st}f'(t)|_{0}^\infty-(-s)\int_{0}^{\infty} e^{-st}f'(t) \, dt $$
$$=-f'(0)+s(sF(s)-f(0))$$
$$=s^sF(s)-sf(0)-f'(0)$$
$$\mathcal{L}(f^{n}(t))=s^nF(s)-s^{n-1}f(0)$$
##### 5.
$$\mathcal{L}\left( \int_{0}^{t} f(\tau) \, d\tau  \right)$$
Let $g(t)=\int_{0}^{t} f(\tau) \, d\tau, g(0)=0$
$$g'(t)=f(t)$$
$$\mathcal{L}(g'(t)) = \mathcal{L}(f(t))=F(s)$$
$$G(s)=\frac{F(s)}{s}$$
$$\mathcal{L}\left( \int_{0}^{t} f(\tau) \, d\tau  \right) = \frac{F(s)}{s}$$
---
###### 6.
L.T of powers of t: $f(t) = t^n$
$$\mathcal{L}(t)= \int_{0}^{\infty} e^{-st}t \, dt $$
$$=\frac{e^{-st}}{-s}t|_{0}^\infty+\frac{1}{s}\int_{0}^{\infty} e^{-st}1 \, dt $$
$$\mathcal{L}(t) = \frac{1}{s^2}$$
$$\mathcal{L}(t^2) = \int_{0}^{\infty} e^{-st}t^2 \, dt $$
$$\frac{e^{-st}}{-s}t^2|_{0}^\infty+\frac{2}{s}\int_{0}^{\infty} e^{-st}t \, dt $$
$$=\frac{2}{s^3}$$
$$\mathcal{L}(t^n) = \frac{n!}{s^{n+1}}$$
###### 7.
$$\mathcal{L}(\cos/\sin (at))$$
Recall $e^{iat} = \cos (at)+i\sin(at+)$
$$\mathcal{L}(e^{iat})=\int_{0}^{\infty} e^{-st}e^{iat} \, dt $$
$$=\int_{0}^{\infty} e^{-(s-ia)t} \, dt $$
$$=\frac{s}{s^2+a^2}+i \frac{a}{s^2+a^2}$$
$$\mathcal{L}(\cos at) = \frac{s}{s^2+a^2}, \mathcal{L}(\sin at) = \frac{a}{s^2+a^2}$$
EG:
$$m\dot{x}\dot{} + kx = F_{0}\cos\omega t$$
$$\dot{x}\dot{} + \omega_{0}^2x = \gamma \cos\omega t$$
$$\omega_{0} = \sqrt{ \frac{k}{m} }$$
$$\gamma = \frac{F_{0}}{m}$$
$$x(0) = 0 = \dot{x}(0)$$
$$s^2X(s)-sx(0)-\dot{x}(0) + \omega_{0}^2X(s)=\gamma\left( \frac{s}{s^2+a^2} \right)$$
$$(s^2+\omega_{0}^2)=X(s)=\gamma\left( \frac{s}{s^2+\omega_{0}^2} \right)$$