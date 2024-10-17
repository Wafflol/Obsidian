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
