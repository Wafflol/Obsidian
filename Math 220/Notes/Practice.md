a.
{0, 1, 4, 9, 16,...}
b.
{$\sqrt{ 2 }, -\sqrt{ 2 }$}
c.
{}
d.
$[0,9)$
e.
$\{{\frac{1}{7}, \frac{1}{8}, \frac{1}{9},\dots}\}$

2.
a.\
A = $\{x\in \mathbb{Z}|4x\}$
B = $\{3x| x\in \mathbb{Z}\}$
b.
C = $\{x \in \mathbb{Z}\}$
c.
yes

P: $6| n$
Q: $10 | n$
R: $2|n$
$Q \lor P \Rightarrow R$
Contrapositive:
$$\sim R \Rightarrow (\sim Q) \land (\sim P)$$
for $n \in \mathbb{Z}$, if $n$ is not divisible by 2, then $n$ is not divisible by 6 and not divisible by 10

Converse:
$$R \Rightarrow Q \lor P$$
for $n \in \mathbb{Z}$, if $n$ is divisible by 2, then $n$ is divisible by 6 or 10


6.
scratch
$$P\Rightarrow Q \equiv \sim P \lor Q$$
$$(\sim P\lor Q) \Rightarrow R \equiv \sim(\sim P\lor Q)\lor R$$
$$(P\land \sim Q)\lor R$$
$$\Rightarrow (P \lor R) \land (\sim Q \lor R)$$
$$\Rightarrow (P \lor R) \land (Q\Rightarrow R)$$
$$\Rightarrow \sim(P\lor R) \lor \sim(Q\Rightarrow R)$$
$$\Rightarrow (P\lor R) \Rightarrow \sim(Q\Rightarrow R)$$

Prove the statement: $n\in\mathbb{Z}$ $n \equiv 3 (\text{mod} 5)$ iff $5 | (3n+1)$
$$n \equiv 3 (\text{mod }5)$$
$$\Rightarrow n = 3+ 5k \text{ where } k\in Z$$
$$\frac{3n+1}{5} = k, k\in \mathbb{Z}$$
let $k = 2n$
$$n = 3 + 10n$$
$$\Rightarrow 9n= -3$$
$$ \Rightarrow n = -\frac{1}{3}$$
___
Answer: Proof
$$n \equiv 3 (\text{ mod } 5) \Rightarrow 5 | (3n+1):$$
$$n = 3 + 5k, k \in \mathbb{Z}$$
$$3n = 9 + 15k$$
$$3n+1 = 10+15k$$
$$= 5(2+3k)$$
since $k \in \mathbb{Z}$, we have $(2+3k) \in \mathbb{Z}$, so $5 | (3n+1)$

___
$$5 | (3n+1) \Rightarrow n \equiv 3 (\text{mod 5}):$$
$$3n+1 = 5m, \text{for some } m \in \mathbb{Z}$$
$$9n + 3 = 15m$$
$$(10n  -n) + 3 = 15m$$
$$10n+3 -15m = n$$
$$3 + 5(2n-3m) = n$$
since $n, m \in \mathbb{Z}$ we have $(2n-3m) \in \mathbb{Z}$, so $n \equiv 3 \text{ (mod 5)}$
___

Prove:
$a, b \in \mathbb{R}$
if $a\neq b$, then $\frac{a+b}{2}>a$ or $\frac{a+b}{2}>b$
$\left( a\neq b \Rightarrow \frac{a+b}{2} > a \right) \lor (a\neq b \Rightarrow \frac{a+b}{2} >b)$ 
___
$$\begin{align}
\left( (a=b) \lor \frac{a+b}{2}>a \right) \lor \left( (a=b) \lor \frac{a+b}{2}>b \right) \\

\end{align}$$
___
scratch:
$$\begin{align}
\frac{a+b}{2} &> a \\
a+b &> 2a \\
b &> a \\
\end{align}$$

$$\begin{align}
\frac{a+b}{2} &> b \\
a+b &> 2b \\
a &> b
\end{align}$$
___
proof:
Assume $a\neq b$
Then either $a>b$ or $b>a$
Case 1$(a>b):$
$$\begin{align}
a &> b \\
a + b &> 2b \\
\frac{a+b}{2} &> b
\end{align}$$
Case 2 ($b>a$): 
same shit

Therefore the implication holds. $\square$

---
$$x \in \mathbb{R}$$
prove contrapositive
$$x^{1/3} = \frac{p}{q}, p,q\in \mathbb{Z}$$
$$x=\frac{p^3}{q^3}$$
since $\frac{p^3}{q^3} \in \mathbb{Z}$, x is rational
thus, the implication is true

---
let $x>0$
assume $x-\frac{3}{x}> 2$
$$x^2-3>2x$$
$$x^2-2x-3>0$$ (since $x>0$)
$$(x-3)(x+1)>0$$
we will solve by cases
Case 1: $x > 3$
since $x-3 >0$ and $x+1 > 0$
thus, because a positive number multiplied by another positive number is positive, $(x-3)(x+1)>0$
Case 2: $0<x<3$
womp womp
Case 3: $x = 3$
womp womp

Thus, the implication is true

---
assume $n\in\mathbb{Z}$
Proof by cases:
Case 1: $n$ is even
$$n = 2k, k \in \mathbb{Z}$$
$$n^2+3n+8=4k^2+6k+8$$
$$=2(2k^2+3k+4)$$
Since $2k^2+3k+4\in\mathbb{Z}$, $n^2+3n+8$ is even
Case 2: $n$ is odd
$$ n = 2l + 1, l \in \mathbb{Z}$$
$$n^2+3n+8 = 4l^2+4l+1+6l+3+8$$
$$=2(2l^2+5l+6)$$
since $2l^2+5l+6 \in \mathbb{Z}$, $n^2+3n+8$ is even

in both cases, $n^2+3n+8$ is even. Thus, the implication is true.

---


assume $n \in \mathbb{Z}$
Case 1: $n = 3k, k \in \mathbb{Z}$
$$2n^2+n+1=18k^2+3k+1$$
$$=3(6k^2+k)+1$$
since $k \in \mathbb{Z}$, then $6k^2+k \in \mathbb{Z}$, and thus, $3 \nmid 3(6k^2+k)+1$ 
Case 2: $n = 3k+1, k \in\mathbb{Z}$
$$2n^2+n+1 = 2(9k^2+6k+1)+3k+1+1$$
$$=18k^2+15k+4$$
$$=3(6k^2+5k+1)+1$$
Since $k \in \mathbb{Z}$, $6k^2+5k+1 \in \mathbb{Z}$, and thus, $3 \nmid 3(6k^2+5k+1)+1$ 

Case 3: $n = 3k+2, k\in \mathbb{Z}$
$$2n^2+n+1 = 2(9k^2+12k+4)+3k+2+1$$
$$=18k^2+27k+11$$
$$=3(6k^2+9k+3)+2$$
since $k \in \mathbb{Z}$, $6k^2+9k+3 \in \mathbb{Z}$, and thus, $3 \nmid 3(6k^2+9k+3)+2$

Thus, the implication is true

---

-1, 3
Case 1:
$$x: (-\infty,-1]$$
$x+1$ is negative, so $\mid x+1 \mid = -(x+1)$
$x-3$ is negative, so $|x-3| = -(x-3)$ 
$$-x-1-(-x+3)=-4$$
since $-4=-4$ the implication holds true in this case
Case 2:
$$x: (-1,3)$$

Case 3:
$$x: [3,\infty)$$


---

$$\forall z > 0, \mid x - y \mid < z \Rightarrow (x=y)$$
$$(\exists z > 0, \mid x-y \mid \geq z) \lor (x = y)$$
---


Show that $\lim_{ x \to 1 }(5x+3) = 8$
$$\forall \epsilon > 0, \exists \delta > 0 \text{ } s.t. \text{ } 0 < \mid x - c \mid < \delta \Rightarrow \mid f(x) - L \mid  < \epsilon$$

need to show that $0 < \mid x - 1 \mid < \delta \Rightarrow \mid (5x+3)-8 \mid < \epsilon$

$$\mid  5x-5 \mid < \epsilon$$
$$\mid x-1 \mid < \frac{\epsilon}{5}$$
formal proof:
Proof:
Given $\epsilon > 0$ , let $\delta = \frac{\epsilon}{5}$
If $0 < \mid x - 1 \mid < \delta = \frac{\epsilon}{5}$, 
then $\mid x-1 \mid < \frac{\epsilon}{5}$
$$\Rightarrow 5 \mid x-1 \mid  < \epsilon$$
$$\Rightarrow \mid 5x-5 \mid  < \epsilon$$
$$\Rightarrow \mid (5x+3)-8 \mid < \epsilon$$
so $\lim_{ x \to 1 }(5x+3)=8$


___


$$\forall \epsilon > 0, \exists \delta > 0 \text{ } s.t. \text{ } 0 < \mid x - c \mid < \delta \Rightarrow \mid f(x) - L \mid  < \epsilon$$


$$\lim_{ x \to 2 } \left( \frac{1}{x} \right)=\frac{1}{2}$$
$$0 < \mid x-2 \mid < \delta \Rightarrow \mid \frac{1}{x} - \frac{1}{2} \mid < \epsilon$$
$$\mid  \frac{2-x}{2x} \mid < \epsilon$$
$$\mid x-2 \mid  < \epsilon * 2 \mid x \mid $$
---
Proof:
Given $\epsilon > 0$, let $\delta = min{1, 2\epsilon}$
If $0 < \mid  x - 2 \mid < \delta$
Since $\delta \leq 1$, we have $1 < x < 3$
Since $\delta \leq 2\epsilon$, we have $\mid  x- 2 \mid < 2\epsilon$

---

$$\frac{1}{2}, \frac{1.5}{2.5}, \frac{1+\frac{3}{5}}{2+\frac{3}{5}}$$



---

base case: $F_{4} = 3$, $3 \mid F_{4}$
$1, 1, 2, 3, 5, 8, 13, 21, 34$
$3, 21$
$F_{5} = F_{4} + F_{3} = 3 + 2 = 5$
$F_{6} = F_{5} + F_{4} = 5 + 3 = 8$
$F_{7} = F_{6} + F_{5} = 8 + 5 = 13$
$F_{8} = F_{7} + F_{6} = 13 + 8 = 21$

assume $F_{4n} = 3k, k \in \mathbb{Z}$
$$F_{4n}=3k$$
$$F_{4n+4} = F_{4k+3}+F_{4k+2}=F_{4k+2}+F_{4k+1}+F_{4k+1}+F_{4k}$$
$$=F_{4k+1}+F_{4k}+F_{4k+1}+F_{4k+1}+F_{4k}$$
$$=3F_{4k+1}+2F_{4k}$$
$$3F_{4k+1}+6k$$
$$=3(F_{4k+1}+2k)$$
---
$$a_{1} = 1$$

Let $a_{n}=2n-1$ for $n \in \mathbb{N}$
When $n = 2$, $a_{n} = 3 = 2n-1$
$a_{n+1}=2n+1=2a_{n}-a_{n-1}$ for $n \geq 3$
$$\begin{align}
2n+1&=2(2n-1)-a_{n-1}  \\
2n + 1 &= 4n-2-a_{n-1} \\
6n+3 &= -a_{n-1} \\

\end{align}$$
---
$$a_{n+2} = 2a_{n+1} - a_{n}$$
$$=2(2(a_{n})-a_{n-1}) -(2n-1)$$
$$=4(2n-1)-2a_{n-1}-(2n-1)$$
$$=3(2n-1)-2a_{n-1}$$


$$a_{n}=2n-1 \Rightarrow a_{n+1} = 2n+2 $$
---

$$0, \{ 1 \}, \{ 2 \} \{ 1,2 \}$$
$$\{ \{ 2 \}, \{ 1,2 \} \}$$
$$\{ \{  \}, \{ \{ 2 \} \}, \{ \{ 1,2 \} \}, \{ \{ 2 \}, \{ 1,2 \} \} \}$$
$$$$

---

$$a R b \Rightarrow 6a^2 \equiv 2b^2 (\text{ mod 5 })$$
$$a R a \Rightarrow 7a^2 \equiv 2a^2 (\text{mod 5})$$
$$7a^2 =2a^2+ 5a^2$$
$$= 2a^2+5(a^2)$$
Since $a^2 \in \mathbb{Z}$, then it follows that the relation is reflexive

$$aRb \Rightarrow 7a^2\equiv 2b^2$$
$$7a^2 \equiv 2b^2 (\text{mod 5}) \Rightarrow 7b^2 \equiv 2a^2 (\text{mod 5})$$

---

Reflexive: 
$\forall a \in A$ we have $a Ra$ since $a$ is in the same $S \in P$ as itself.
Symmetric
If $a R b$ for some $a, b, \in A$, then $a, b \in S$, for some $S \in P$.
Then $b, a \in S$, so $b R a$
Transitive:
If $a R b$  and $b R c$, for some $a, b, c, \in A$, then $\exists S_{1}, S_{2} \in P$ such that $a, b, \in S$ and $b, c, \in S_{2}$.
Since $S_{1} \cap S_{2} \neq \{\}$ (since $b \in S_{1} \cap S_{2}$), the $S_{1} = S_{2}$ (since $P$ is a partition). So $a, b, c, \in S_{1}$ so $aRc$





