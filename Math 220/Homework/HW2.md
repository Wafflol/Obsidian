1.
===
Prove that if $a \in \mathbb{Z}$, then $4 \nmid a^2 + 1$
Proof by cases
Case 1: $a = 4n, \text{ } n \in \mathbb{Z}$
$$\begin{align} 
a^2 +1 &= 
(4n)^2+1\\&=16n^2+1\\ 
&= 4(4n^2)+1
\end{align}$$
Since $n \in \mathbb{Z}$, then $4n^2 \in \mathbb{Z}$, so $4 \nmid 4(4n^2)+1$ 

Case 2: $a = 4n + 1 \text{ } n \in \mathbb{Z}$
$$\begin{align}
a^2+1&= (4n+1)^2+1  \\
&= 16n^2+8n+2 \\
&= 4(4n^2+2n)+2
\end{align}$$
Since $n \in \mathbb{Z}$, then $4n^2+2n \in \mathbb{Z}$, so $4 \nmid 4(4n^2+2n)+2$

Case 3: $a = 4n + 2 \text{ } n \in \mathbb{Z}$
$$\begin{align}
a^2+1 &= (4n+2)^2+1 \\
&=16n^2+16n+5 \\
&=4(4n^2+4n+1)+1
\end{align}$$
Since $n \in \mathbb{Z}$, then $4n^2+4n+1 \in \mathbb{Z}$, so $4 \nmid 4(4n^2+4n+1)+1$

Case 4: $a = 4n + 3 \text{ } n \in \mathbb{Z}$
$$\begin{align}
a^2+1 &= (4n+3)^2+1  \\
&= 16n^2 + 24n + 10 \\
&= 4(4n^2+6n+2)+2
\end{align}$$
Since $n \in \mathbb{Z}$, then $4n^2+6n+2 \in \mathbb{Z}$, so $4 \nmid 4(4n^2+6n+2)+2$

Thus, due to proof by cases, the implication is true.

2.
===
Let $k \in \mathbb{Z}$
Prove $3 \mid k(2k+1)(4k+1)$
Proof by cases:
Case 1: $k = 3n, \text{ } n \in \mathbb{Z}$
$$\begin{align}
k(2k+1)(4k+1) &= 3n(6n+1)(12n+1) \\
&= 3(n(6n+1)(12n+1))
\end{align}$$
Since $n \in \mathbb{Z}$, that means that $(n(6n+1)(12n+1)) \in \mathbb{Z}$, so $3 \mid 3(n(6n+1)(12n+1))$, and therefore $3 \mid k(2k+1)(4k+1)$

Case 2: $k = 3n + 1, \text{ } n \in \mathbb{Z}$
$$\begin{align}
k(2k+1)(4k+1) &= (3n+1)(6n+3)(12n+5)  \\
&= 3((3n+1)(2n+1)(12n+5))
\end{align}$$
Since $n \in \mathbb{Z}$, that means that $(3n+1)(2n+1)(12n+5) \in \mathbb{Z}$, so $3 \mid 3((3n+1)(2n+1)(12n+5))$, and therefore $3 \mid k(2k+1)(4k+1)$

Case 3: $k = 3n + 2, \text{ } n \in \mathbb{Z}$
$$\begin{align}
k(2k+1)(4k+1) &= (3n+2)(6n+5)(12n+9)  \\
&= 3((3n+2)(6n+5)(4n+3))
\end{align}$$
Since $n \in \mathbb{Z}$, that means that $(3n+2)(6n+5)(4n+3) \in \mathbb{Z}$, so $3 \mid 3((3n+2)(6n+5)(4n+3))$, and therefore $3 \mid k(2k+1)(4k+1)$

Thus, due to proof by cases, the implication is true.

3.
===
Let $n \in \mathbb{Z}$
a.
---
Prove $3 \mid n \land 4 \mid n \Rightarrow 1 2\mid n$
Let $n = 3m \land n = 4l, m,l \in \mathbb{Z}$
Using Bezout’s identity, which is:
Let $a, b, \in \mathbb{Z}$ such that $a$ and $b$ are not both zero. Then there exists $x, y, \in\mathbb{Z}$ such that $ax+by=gcd(a,b)$
Thus, if we let $a = 3$, and $b = 4$, and $m = x, l = y$
we get $\exists m, l, \in\mathbb{Z} \text{s.t.}$$3m+4l = gcd(a,b) = 1$ when $m = -1, l = 1$
Using the definition of lcm, $lcm(a,b) = \frac{\mid ab \mid}{gcd(a,b)}$
thus, $lcm(4,3) = 12$, and so it follows that $12 \mid n$
Thus, by proving the contrapositive, we find that the implication is true.

b.
---
If $n > 3$ is prime, then $n^2 \equiv 1 (\text{mod } 12)$
Let $n > 3$
Proof by cases:
As $n$ is prime,  




---


4.
===
Let $n \in \mathbb{Z}$
Prove $$3\mid n^3 + n^2 - n +3 \Rightarrow 3 \mid n$$
Contrapositive:
$$3 \nmid n \Rightarrow 3 \nmid n^3+n^2-n+3$$
$$n \neq 3k, k \in \mathbb{Z}$$
Since $n \neq 3k$, there are two cases of $n$
Proof by cases: 
Case 1: $n = 3k+1$
$$\begin{align}
n^3+n^2-n+3&=27k^3+36k^2+12k+4 \\
&= 3(9k^3+12k^2+4k+1)+1
\end{align}$$
Since $9k^3+12k^2+4k+1 \in \mathbb{Z}$, using the division algorithm, it follows that $3 \nmid 3(9k^3+12k^2+4k+1)+1$, and thus, $3 \nmid n^3+n^2-n+3$ in this case.

Case 2: $n = 3k+2$
$$\begin{align}
n^3+n^2-n+3 &= 27k^3+63k^2+45k+13 \\
&= 3(9k^3+21k^2+15k+4)+1
\end{align}$$
In similar fashion, since $9k^3+21k^2+15k+4 \in \mathbb{Z}$, if follows that $3 \nmid 3(9k^3+21k^2+15k+4)+1$. Thus, $3\nmid n^3+n^2-n+3$ in this case.

Therefore, using proof by cases on the contrapositive, $3\nmid n^3+n^2-n+3$, and the implication is true.


5.
===
Let $x \in \mathbb{R}$
Proof by cases:
Case 1: $x\geq6$
$$\begin{align}
x^2+(x-6) &= x^2+x-12+6 \\
&=(x+4)(x-3)+6
\end{align}$$
Since $x\geq 6$, $(x+4),(x-3)>0$ and $6$ plus any positive number is always greater than 5.

Case 2: $x < 6$
$$\begin{align}
x^2-(x-6) &= x^2-x+6 \\
&=\left( x-\frac{1}{2} \right)^2+\frac{23}{4} \\
\end{align}$$
Since $\left( x-\frac{1}{2} \right)^2 >0$ and $\frac{23}{4} > 5$, in this case, $x^2+\mid x-6 \mid >5$
Thus, using proof by cases, it follows that $x^2 + \mid x-6 \mid > 5$, and thus, the implication is true
6.
===
Let $x, y \in \mathbb{Z}$
Prove $$3 \nmid(x^3+y^3) \iff 3 \nmid(x+y)$$
$$\sim((P\land \sim Q)\lor(\sim P \land Q))$$

---

$$(x+y)(x^2-xy+y^2)=3k$$
 