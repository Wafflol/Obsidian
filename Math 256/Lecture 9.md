### Forced Undamped Oscillations
$$m\dot{x}\dot{} + kx = F_{0}\cos(\omega t)$$
$$x(0)=0, \dot{x}(0)=0$$
$$\dot{x}\dot{} + \omega_{0}^2x=\gamma \cos\omega t$$
$$\omega_{0}=\sqrt{ \frac{k}{m} }$$
$$x_{H}=c_{1}\cos\omega_{0}t+c_{2}\sin\omega t$$
$$\omega \neq \omega_{0}$$
$$x_{p}(t)=A\cos\omega t+B\sin\omega t$$
$$\dot{x}_{p}=-A\omega \sin\omega t+B\omega \cos\omega t$$
$$\dot{x}\dot{}_{p} = -A\omega^2\cos\omega t-B\omega^2\sin\omega t$$
$$\dot{x}\dot{}+\omega^2_{0}x_{p} = \gamma \cos\omega t$$
	$$\dot{x}\dot{}_{p} + \omega^2_{0}x_{p}=A(\omega_{0}^2-\omega^2)\cos\omega t+ B(\omega_{0}^2-\omega ^2)\sin\omega t$$

$$=\gamma \cos\omega t + 0\sin\omega t$$
$$B = 0, A = \frac{\gamma}{\omega^2-\omega^2}$$
General solution
$$x(t)=c_{1}\cos\omega_{0}t+c_{2}\sin\omega_{0}t+ \frac{\gamma}{\omega_{0}^2-\omega^2}\cos\omega t$$
$$\dot{x}(t)=-\omega_{0} c_{1}\sin\omega_{0} t+c_{2}\omega_{0}\cos\omega_{0} t$$
$$0=x(0)=c_{1}+\frac{\gamma}{\omega_{0}^2-\omega^2}\Rightarrow c_{1}= - \frac{\gamma}{\omega_{0}^2-\omega^2}$$
$$0 = \dot{x}(0) = c_{2}\omega_{0}+0 \Rightarrow c_{2}=0$$
$$x(t) = \frac{\gamma}{\omega_{0}^2-\omega^2}(\cos\omega t-\cos\omega_{0}t)$$
---
### trig to remember
$$\cos(\alpha\pm\beta) = \cos\alpha \cos\beta\mp\sin\alpha \sin\beta$$
$$\cos(\alpha-\beta)-\cos(\alpha+\beta)=2\sin\alpha \sin\beta $$
$$\text{Let }\alpha-\beta = \omega t, \alpha+\beta=\omega_{0}t$$
$$\alpha = \frac{(\omega_{0}+\omega)t}{2}, \beta=\frac{(\omega_{0}-\omega)t}{2}$$
