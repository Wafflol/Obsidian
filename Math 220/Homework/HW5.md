1.
Proof by induction:
Base Case: $n = 1$
When $n=1$, 
$$\begin{align}
\sum_{k=1}^{1}(2k-1)2^k = 2 &=  6 + 2^1(4(1)-6) \\
2 & =  6-4 \\
2 &= 2
\end{align}$$
Thus, the base case is true.
Induction step:  assume true for some $k \in \mathbb{N}$
Let $\sum_{k=1}^{n}(2k-1)2^k=6+2^n(4n-6)$
$$\begin{align}
\sum_{k=1}^{n+1} (2k-1)2^k &= \sum_{k=1}^{n}(2k-1)2^k+(2(n+1)-1)2^{n+1} \\
&= 6+2^n(4n-6)+(2n+1)2^{n+1} \\
&= 6 + 2^n 4n - 6*2^n + 2n*2^{n+1} + 2^{n+1} \\
&= 6 + 2n(2^{n+1})+2n(2^{n+1})-3(2^{n+1})+2^{n+1} \\
&= 6 + 4n(2^{n+1}) - 2(2^{n+1}) \\
&= 6 + 2n^{n+1}(4n-2) \\
&= 6 + 2n^{n+1}{(4(n+1)-6})
\end{align}$$
Thus, using proof by induction, it follows that the implication is true.

2.
Proof by induction:
Base Cases: $n = 1$, $n = 2$
When $n = 1$,
$$\begin{align}
a_{1} = 3-2=1
\end{align}$$
When $n = 2$
$$\begin{align}
a_{2} = 3^2-2^2=5
\end{align}$$

Induction Step: assume true for some $k \in N, k \geq2,  \text{ and for } k-1$
Let:
$$\begin{align}
a_{k} = 5a_{k-1}-6a_{k-2} = 3^k-2^k, k\geq 3
\end{align}$$
$$\begin{align}
a_{k+1} &= 5a_{k}-6a_{k-1} \\
&= 5a_{k-1}-6a_{k-2}-6a_{k-1} \\
&= 5(3^k-2^k )- 6a_{k-1} \\
& = 5(3^k -2^k) -6(3^{k-1}-2^{k-1}) \\
&= 5(3^k-2^k )- (2*3^k-3*2^k) \\
&= 3*3^k-2*2^k \\
&= 3^{k+1}-2^{k+1}
\end{align}$$
Thus, using strong induction, it follows that the implication is true

3.
Proof by induction:
Base Cases: $n = 1$, $n = 2$
When $n=1$, 
$$f_{2}f_{0}-f_{1}^2= (f_{1}+f_{0})(0)-1^2=-1=(-1)^1$$
When $n =2$,  
$$f_{3}f_{1}-f_{2}^2=(f_{1}+f_{0}+f_{1})f_{1}-(f_{1}+f_{0})^2=(2-1)=1=(-1)^2$$
The implication holds for the base case
Induction Step: assume true for some $k \in \mathbb{N}$
Let $f_{k+1}f_{k-1}-f^2_{k}=(-1)^k$ for $k \geq 2$
Then $f_{k}^2=f_{k+1}f_{k-1}-(-1)^k$

Let k = 3
$$\begin{align}
f_{k+2}f_{k}-f_{k+1}^2&=(f_{k+1}+f_{k})f_{k}-(f_{k+1})^2 \\
&= f_{k+1}f_{k}+f_{k}^2 - f_{k+1}^2 \\
&= -f_{k+1}(f_{k+1}-f_{k})+f_{k}^2 \\
&= -f_{k+1}(f_{k}+f_{k-1}-f_{k})+f_{k}^2 \\
&= -f_{k+1}(f_{k-1})+f_{k}^2 \\
&= -f_{k+1}(f_{k-1}) + f_{k+1}f_{k-1}-(-1)^k \\
&= -1*(-1)^k \\
&= (-1)^{k+1}
\end{align}$$
Thus, using proof by induction, it follows that the implication holds true.

4.
Proof by induction:
Base Cases: $n = 1$, $n = 0$
When $n = 1$
$$\begin{align}
7^{4+3}+2 &= 823543+2 = 823545 \\
&= 5 (164709)
\end{align}$$

By Euclidian division, $5 \mid 5*164709$, and thus, this base case holds true.

When $n = 0$
$$\begin{align}
7^3+2 &= 343+2 = 345 \\
&= 5(69)
\end{align}$$
By Euclidian division, $5 \mid 5*69$, and thus, both base cases hold true.

Induction step: assume true for some $k \in \mathbb{N}$
Let $7^{4k+3}+2 \equiv 0 ( \text{ mod 5})$
It follows that $7^{4k+3} \equiv 3 \text{ (mod 5) }$
and thus, $7^{4k+3}=3+5l$ for some $l \in \mathbb{Z}$
$$\begin{align}
7^{4(k+1)+3}+2 &= 7^{4k+7}+2 \\
&= 7^{4k+3} \cdot 7^{4}+2 \\
&= 3+5l \cdot  7^4 + 2, l \in \mathbb{Z} \\
&= 5 + 5l \cdot 7^4 \\
&= 5(1+7^4l)
\end{align}$$
Since $1+7^4l \in \mathbb{Z}$, then it follows that $5 \mid 5(1+7^4l)$, and thus, using proof by induction, the implication holds true.

5.
Proof by induction:
Base Cases: $n = 0, n = 1$
When $n = 0$,
$$\begin{align}
u_{0} = \cos(0) = 1
\end{align}$$
When $n = 1$,
$$\begin{align}
u_{1} = \cos(x * 1) = \cos x
\end{align}$$
In both base cases, the implication holds true.
Induction step: assume true for some $k \in \mathbb{N}$, $k \geq 2$, and for $k = n-1$
Let:
$$\begin{align}
u_{k} &= 2u_{1}u_{k-1}-u_{k-2} = \cos(kx) \\
u_{k-1} &= 2u_{1}u_{k-2}-u_{k-3}=\cos(kx-x)
\end{align}$$
Then,
$$\begin{align}
u_{k+1} &= 2u_{1}u_{k}-u_{k-1} \\
&=2\cos (x) (\cos(kx)) -  \cos(kx-x) \\
&= 2\cos x\cos(kx) - (\cos(kx)\cos(x)+\sin(kx)\sin(x)) \\
&= \cos x\cos(kx)-\sin x\sin(kx) \\
&= \cos(x+kx)
\end{align}$$
Thus, using proof by induction, it follows that the implication is true.

6.
Using the original equation, $n^3>2n^2+n$, we can rearrange it to get the following:
$$\begin{align}
n^3-2n^2-n &> 0 \\
n(n^2-2n-1) &> 0 \\
\end{align}$$
Finding the roots of the inner function, $n^2-2n-1$, using the quadratic formula we get the roots $n = 1 \pm \sqrt{ 2 }$. 
Since we only care about positive $n$ values, we can ignore the roots, $n = 1-\sqrt{ 2 }, 0$.
This leaves only one zero of the function, $n = 1+\sqrt{ 2 }$. Thus, as a continuous function like $n^3-2n^2-n$ can only change signs at a zero, we can check which side of the function it's positive. Plugging in a number $l = 3 > 1+\sqrt{ 2 }$, it follows that $l^3-2l^2-l = 6 >0$. Plugging in a number $m = 1 < 1+ \sqrt{ 2 }$, it follows that $m^3-2m^2-m = -2 < 0$. Plugging in a number $j = 2 < 1 + \sqrt{ 2 }$, it follows that $j^3-2j^2-j=-2 < 0$.
Thus, it follows that the implication does not hold for the values $n = 1, 2$, but it holds true for $n = 3$.

Proof by induction:
Since the implication holds true for $n = 3$, it acts as the base case:
When $n = 3$,
$$\begin{align}
n^3 &> 2n^2 +n \\
27 &> 18 + 3 \\
27 &> 21
\end{align}$$
This shows, once again that the implication holds true for the base case $n = 3$.
Induction step:  assume true for some $k \in \mathbb{N}$, for $k \geq 3$
Let: 
$$\begin{align}
k^3 > 2k^2 + k
\end{align}$$
Then,
$$\begin{align}
(k+1)^3 &= (k+1)^2k+(k+1)^2 \\
&= k(k+1)^2+k(k+1)+k+1 \\
\end{align}$$
Since $k\geq 3$, it follows that $k(k+1)^2+k(k+1)+k+1 > 2(k+1)^2 +(k+1)$, and thus, by proof by induction, it follows that the implication is true.