##### Newton's Law of Cooling
$$\frac{dT}{dt} = -k(T-T_{a}(t))$$

----
### Practice
Car windshield being heated

$$T_{a}(t)=T_{\infty}$$
$$T(0) = T_{\infty}$$
$$\frac{dT}{dt}=\text{heat in heat out}$$
$$=n-k(T(t)-T_{\infty})$$
$$\frac{dT}{dt}+kT=n+kT_{\infty}$$
$$F=e^{kt}: e^{kt} \frac{dT}{dt}+ke^{kt} T = (n+kT_{\infty})e^{kt}$$
$$\frac{d}{dt}[e^{kt}T]=(n+kT_{\infty}e^{kt})$$
$$e^{kt}T=(n+kT_{\infty}) \frac{e^{kt}}{k}+c$$
$$T=\frac{n}{k}+T_{\infty}+ce^{-kt}$$
$$T(0)=T_{\infty}=\frac{n}{k}+T_{\infty}+c \Rightarrow c=-\frac{n}{k}$$
$$T(t) = T_{\infty} + \frac{n}{k}(1-e^{-kt})$$
Solve for time
$$0 = T(t_{0})= T_{\infty}+\frac{n}{k}(1-e^{-kt}))$$
