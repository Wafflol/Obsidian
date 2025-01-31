$$\mathcal{L}(f(t))(s)=F(s):=\int_{0}^{\infty} e^{-st}f(t) \, dt $$
$$\mathcal{L}(t^k)=\frac{k!}{s^{k+1}}$$
##### First Shift Theorem
$$\mathcal{L}(e^{at}f(t))=\int_{0}^{\infty} e^{-st}e^{at}f(t) \, dt $$
$$=\int_{0}^{\infty} e^{-(s-a)t}f(t) \, dx $$
$$=F(s-a)$$
---
Eg1
$$Y(s)=\frac{1}{s+a}=\frac{1}{s-(-a)}$$
$$y(t)=\mathcal{L}^{-1}(Y(s))=e^{-at}1$$
2.
$$Y(s)=\frac{2s+3}{s^2+4}$$
$$=2\left( \frac{s}{s^2+2^2} \right)+\frac{3}{2}\left( \frac{2}{s^2+2^2} \right)$$
$$y(t)=2\cos(2t)+\frac{3}{2}\sin(2t)$$
3.
$$Y(s)=\frac{4}{s^2+2s+5}$$
$$=\frac{4}{(s+1)^2+4}$$
$$=2\left( \frac{2}{(s+1)^2+4} \right)$$
$$y(t)=2e^{-t}\sin(2t)$$
4.
$$Y(s)=\frac{s+3}{s^2+4s+5}$$
$$=\frac{s+3}{(s+2)^2+1}$$
$$\frac{s+2}{(s+2)^2+1}+\frac{1}{(s+2)^2+1}$$
$$y(t)=e^{-2t}\sin(t)+e^{-2t}\cos(t)$$
5.
Partial Fraction Expansions
Eg.
$$\frac{s^2+3s+4}{((s-1)(s+2)^2+1)}$$
$$=\frac{As+B}{(s+2)^2+1}+\frac{C}{s-1}$$
$$Y(s)=\frac{N(s)}{D(s)}$$
$N$ and $D$ are polynomials with no common factors and the degree of $N$  < degree of $D$
###### Contribution of factor $(s-a)$ of $D(s)$
$$\frac{N(s)}{D(s)}=\frac{A}{s-a}+H(s)$$
$$\lim_{ s \to a } \frac{(s-a)N(s)}{D(s)-D(a)}=A+(s-a)H(s)$$
$$\frac{N(a)}{D'(a)}=A$$
###### Contribution of a repeated factor $(s-a)^m$ of $D(s)$
$$\frac{N(s)}{D(s)}=\frac{A_{m}}{(s-a)^m}+\frac{A_{m-1}}{(s-a)^{m-1}}+\dots+\frac{A_{1}}{s-a}+H(s)$$
$$Q(s)=(s-a)^m \frac{N(s)}{D(s)}=A_{m}+A_{m-1}(s-a)+\dots+A_{1}(s-a)^{m-1}+(s-a)^mH(s)$$
$$Q(a)=A_{m}$$
$$Q'(a)=A_{m-1}$$
$$Q''(a)=2A_{m-2}$$
$$Q^{k}(a)=k!(A_{m-k})$$
5.
$$Y(s)=\frac{N(s)}{D(s)}=\frac{s-2}{s^2+4s+3}=\frac{s-2}{(s+3)(s+1)}=\frac{A}{s+3}+\frac{B}{s+1}$$
$$D'(s)=2s+4$$
$$A=\frac{N(-3)}{D'(-3)}=\frac{-3-2}{-6+4}$$
$$A=\frac{N(-1)}{D(-1)}=\frac{-1-2}{-2+4}$$
$$y(t)=\frac{5}{2}e^{-3t}-\frac{3}{2}e^{-t}$$
---
Eg6
$$Y(s)=\frac{s+4}{(s+1)(s-4)^2}=\frac{N(s)}{D(s)}$$
$$=\frac{A}{(s-4)^2}+\frac{B}{(s-4)}+\frac{C}{s+1}$$
repeated factor:
$$Q(s)=(s-4)^2 \frac{N(s)}{D(s)}=A+B(s-4)+\frac{C(s-4)^2}{s+1}$$
$$=\frac{s+4}{s+1}$$
$$Q(4)=\frac{8}{5}$$
$$Q'(s)=\frac{(s+1)-(s+4)}{(s+1)^2}$$
$$Q'(4)=\frac{5-8}{25}=\frac{3}{25}$$
$$D(s)=(s+1)(s+1)^2$$
$$D'(s)=(s+4)^2+2(s+1)(s+4)$$
$$c=\frac{N(s)}{D'(s)}|_{s=-1}=\frac{-1+4}{(-5)^2}=\frac{3}{25}$$
$$\frac{8}{5}e^{4t}t-\frac{3}{25}e^{4t}+\frac{3}{25}e^{-t}$$
---
###### Complex Pair of Factors
$$(s-a)(s-\bar{a}) \text{ of } D(s)$$
Let $a=\alpha+i\beta, \bar{a} = \alpha-i\beta$
$$(s-a)(s-\bar{a})=s^2-(a+\bar{a})+a\bar{a}$$
$$a+\bar{a}=2\alpha, a\bar{a}=\alpha^2\beta^2$$
$$(s-a)(s-\bar{a})=s^2-2\alpha s+\alpha^2+\beta^2=(s-\alpha)+\beta^2$$
$$\frac{N(s)}{D(s)}=\frac{As+B}{(s-\alpha^2)+\beta^2}+H(s)$$
$$R(s)=\frac{((s-\alpha)^2+\beta^2)N(s)}{D(s)}=As+B+((s-\alpha)^2+\beta^2)(H(s))$$
$$\mathcal{L}^{-1}\left( \frac{As+B}{(s-\alpha)^2+\beta^2} \right)$$