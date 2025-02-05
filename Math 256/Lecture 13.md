### Laplace Continued
## 1. Scaling
$$\mathcal{L}(f(at))=\int_{0}^{\infty} e^{-st}f(at) \, dt $$
$$=\frac{1}{a}F\left( \frac{s}{a} \right)$$
## 2. Derivatives of $F(s)=\mathcal{L}(f(t))$
$$\frac{d^n}{ds^n}F(s)=\frac{d^n}{ds^n}\left( \int_{0}^{\infty} f(t) \, dt  \right)$$
$$=\frac{d^{n-k}}{ds^{n-k}}\int_{0}^{\infty} (-t^k)f(t) \, dt $$
$$=\mathcal{L}(-t^nf(t))$$
EG:
$$\mathcal{L}(t^3e^{2t})$$
$$g(t)=e^{2t}, G(s)=\frac{1}{s-2}$$
$$\mathcal{L}((-t)^3e^{2t})=\frac{d^3}{ds^3}G(s)$$
$$=-6(s-2)^{-4}$$
$$\mathcal{L}(t^3e^{2t})=\frac{6}{(s-2)^4}$$
EG:
$$y''+\omega_{0}^2y=\gamma \cos\omega_{0}t$$
$$y(0)=0=y'(0)$$
$$\omega_{0}=\sqrt{ \frac{k}{m} }, \gamma=\frac{F_{0}}{m}$$
$$\mathcal{L}: (s^2Y(s)-sy(0)-y'(s))+\omega_{0}^2Y(s)=\gamma  \frac{s}{s^2+\omega_{0}^2}$$
$$Y(s)=\frac{\gamma s}{(s^2+\omega_{0}^2)^2}$$
Now $\mathcal{L^{-1}}\left( \frac{\omega_{0}}{s^2+\omega_{0}^2} \right)=\sin\omega_{0}t$
$$g(t)=\sin\omega_{0}t$$
$$\mathcal{L}(g)=\frac{\omega_{0}}{s^2+\omega_{0}^2}=G(s)$$
$$\frac{dG}{ds}=-\frac{\omega_{0}2s}{(s^2+\omega_{0}^2)^2}=\mathcal{L}(-t\sin\omega_{0}t)$$
$$y(t)=\frac{F_{0}t}{2m\omega_{0}}\sin\omega_{0}t$$
#### Forcing functions with jumps
Heaviside step function
$$u(t) = \begin{cases}
0 & t<0 \\
1 & t\geq 0
\end{cases} = H(t)$$
##### Shifted step
$$u(t-c)=\begin{cases}
1 & t\geq c \\
0 & t<c
\end{cases}$$
$$\mathcal{L}(u(t-c))=\int_{0}^{\infty} e^{-st}u(t-c) \, dt $$
$$=\int_{c}^{\infty} e^{-st} \, dt $$
$$=\frac{e^{-st}}{-s}\mid_{c}^\infty$$
$$\mathcal{L}(u(t-c))=\frac{e^{-sc}}{s}$$
$$\mathcal{L}(u(t-c)f(t-c))=\int_{0}^{\infty} e^{-st}u(t-c)f(t-c) \, dt $$
$$=\int_{c}^{\infty} e^{-st}f(t-c) \, dt $$
$$=\int_{0}^{\infty} e^{-s(\tau+c)}f(\tau) \, d\tau $$
$$\mathcal{L}(u(t-c)f(t-c)=e^{-sc}F(s))$$