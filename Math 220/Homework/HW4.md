1.
Assume $a \mid bc$
$$bc = an, n \in \mathbb{Z}$$
Since $gcd(a,b) = 1$, by Bezout's identity, there exists an $x, y \in \mathbb{Z}$ such that $ax+by=gcd(a,b)=1$.
Let $c \in \mathbb{Z}$, multiply both sides of the equation by c.
$$\begin{align}
ax + by &= 1 \\
cax + cby &= c
\end{align}$$
Stated earlier, since $bc = an$, $bc$ can be substituted by $an$ in the equation above.
$$\begin{align}
cax+any&=c  \\
a(cx+ny)&= c
\end{align}$$
Since $cx+ny$ is an integer, it follows that $a \mid c$. Thus, the implication is true.

---
2.
1.
Pick $x = 3, y = 5$. Since $x+y = 3+5 = 8 \not\in P$, it follows that the implication is false.
2.
Prove the negation:
$$\exists x \in P \text{ } s.t. \text{ } \forall y \in P, x+y \not\in P$$
Let $x = 7$
Case 0: $y \equiv 0 \text{ (mod 2)}$
Since the only even number in $P$ is 2,
$$\begin{align}
x + y &= 2 + 7 \\
&=  9
\end{align}$$
Since $9 = 3(3)$, $3 \mid 9$, and thus, $x+y \not\in P$

Case 1: $y \equiv 1 \text{(mod 2)}$
$$\begin{align}
x+y &= 7 + 1 + 2n, n \in \mathbb{Z} \\
&= 8 + 2n \\
&= 2(4+n)
\end{align}$$
Since $4+n \in \mathbb{Z}$, $2 \mid 4+n$, and thus, it follows that $x+y \not\in P$, and thus, the implication is true for the negation. 
Since the negation is true, that means that the original implication is false.

3.
Negation:
$$\forall x \in P, \exists y \in P \text{ } s.t. \text{ } x+y \not\in P$$
Proving the negation:
Case 0: $x \equiv 1 \text{(mod 2)}$
Pick $y = 3$
$$\begin{align}
x &= 1 + 2n, n \in \mathbb{Z} \\
x+y &= 3+1+2n \\
&= 4 + 2n \\
&= 2(2+n)
\end{align}$$
Since $2+n \in \mathbb{Z}$, it follows that $2 \mid 2+n$, and thus, $x+y \not\in P$

Case 1: $x \equiv 0 \text{(mod 2)}$
Pick $y = 2$
$$\begin{align}
x &= 2n, n \in \mathbb{Z} \\
x + y &= 2n + 2 \\
&= 2(n+1)
\end{align}$$
Since $n+1 \in \mathbb{Z}$, it follows that $2 \mid n+1$, and thus, $x + y \not\in P$.
Thus, by proof by cases, it follows that the negation is true, which means that the original implication is false.

4.
Pick $x = 2, y = 3$. Since $x+y = 5$, and $5 \in P$, $x+y = 5 \in P$. Thus, the implication is true.

3.
Definition of limit:

