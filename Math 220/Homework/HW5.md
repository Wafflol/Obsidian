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
Base Case: $n = 1$, $n = 2$
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
Base Case: $n = 1$, $n = 2$
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
Base Case: $n = 1$
$$\begin{align}
7^{4+3}+2 = 823543+2 = 823545
&= 5 (164709)
\end{align}$$
By Euclidian division, $5 \mid 164709$, and thus, the base case holds true.

Induction step: assume true for some $k \in \mathbb{N}$
Let $7^{4k+3}+2 \equiv 0 ( \text{ mod 5})$
It follow that $7^{4k+3} \equiv 3 \text{ (mod 5) }$
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
