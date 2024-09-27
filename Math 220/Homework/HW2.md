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
Contrapositive:
$$12 \nmid n \Rightarrow 3 \nmid n \lor 4 \nmid n$$
$$n \neq 12k, \text{ } k \in \mathbb{Z}$$
$$n \neq 3(4k)$$
Since $k \in \mathbb{Z}$, then it follows that $4k \in \mathbb{Z}$, which means that $3 \nmid n$.
Thus, by proving the contrapositive, we find that the implication is true.

---
scratch:
$$n = 12k, k \in \mathbb{Z}$$
$$n = 4(3k)$$
b.
---
If $n > 3$ is prime, then $n^2 \equiv 1 (\text{mod } 12)$
Let $n > 3$
Contrapositive:
$$n^2 \neq 1 +12k \Rightarrow n \text{ is not prime}, k \in \mathbb{Z}$$
$$$$


---


4.
===
Let $n \in \mathbb{Z}$
Prove $$3\mid n^3 + n^2 - n +3 \Rightarrow 3 \mid n$$



5.
===
Let $x \in \mathbb{R}$
Proof by cases:


6.
===
Let $x, y \in \mathbb{Z}$
Prove $$3 \nmid(x^3+y^3) \iff 3 \nmid(x+y)$$
$$\sim((P\land \sim Q)\lor(\sim P \land Q))$$
show that the negation is false:
$$3 \mid (x^3 + y^3) \iff 3 \mid (x+y)$$
$$x+y=3k , \text{ } k \in \mathbb{Z}$$

---

$$(x+y)(x^2-xy+y^2)=3k$$
$$$$
