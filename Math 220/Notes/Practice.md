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
