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
Induction step: 
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
a_{1} = 1
\end{align}$$
When $n = 2$
$$\begin{align}
a_{2} = 5
\end{align}$$

Induction Step: assume true for some $n \in N, n \geq2,  \text{ and for } k-1$
Let:
$$\begin{align}
a_{n} = 5a_{n-1}-6a_{n-2} = 3^n-2^n, n\geq 3
\end{align}$$
$$\begin{align}
a_{n+1} &= 5a_{n}-6a_{n-1} \\
&= 5a_{n-1}-6a_{n-2}-6a_{n-1} \\
&= 5(3^n-2^n )- 6a_{n-1} \\
& = 5(3^n -2^n) -6(3^{n-1}-2^{n-1}) \\
&= 5(3^n-2^n )- (2*3^n-3*2^n) \\
&= 3*3^n-2*2^n \\
&= 3^{n+1}-2^{n+1}
\end{align}$$
Thus, using strong induction, it follows that the implication is true

3.
Proof by induction:
Base Case: $n = 1$, $n = 2$
When $n=1$, $$$$
When $n =0, f_{1}=1$
Induction Step:
Let $f_{n+1}f_{n-1}-f^2_{n}=(-1)^n$ for $n \geq 2$
$$\begin{align}
f_{n+1}f_{n-1}-f_{n}^2=(-1)^n = 
\end{align}$$