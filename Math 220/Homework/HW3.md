1.
$$\exists c \in \mathbb{R} \text{ } s.t. \forall \epsilon >0,\exists M >0 s.t. \left|\frac{x^2+\sin(x^2)}{x^2+\cos(x)} -c \right| < \epsilon $$
the negation:
$$\forall c \in \mathbb{R}, \exists \epsilon > 0 s.t. \forall M > 0, \left | \frac{x^2+\sin(x^2)}{x^2+\cos(x)}-c\right| \geq \epsilon$$

2.
$$\exists x \in \mathbb{Z} s.t. \forall y \in \mathbb{R}, \left( x \geq y \land \frac{x}{y} \neq 1\right)$$
Let $x = 0$
$y \in \mathbb{R}$
since $x \geq y$, $y \leq 0$
since $\frac{0}{y}$ is $0$ when $y \neq 0$, and undefined when $y = 0$, the negation of the implication is true, and thus the implication is false.


3.
a.
let $x = 3, y = 3$, $x+y = 6$
Since $3 | 6$, this statement is true

b.
We can first take the negation of this statement:
$$\exists x \in A  \text{ }s.t. \text{ } \exists y \in A \text{ } s.t. \text{ } x+y \not\in A$$
Let $x = 3, y =4, x+y = 7$
Since $3 \nmid 7$ and $4 \nmid 7$, it follows that the negation is true, and thus the implication is false.

c.
We can first take the negation of this statement:
$$\forall x \in A, \exists y \in A \text{ } s.t. x+y \not\in A$$

Proof by cases:
Case 1: $x \equiv 0 \text{( mod 3)}$
$x = 3n, n \in \mathbb{Z}$
Choose $y = 4$
$$\begin{align}
x+y &= 3n + 4 \\
&= 3(n + 1)+1
\end{align}$$
Since $n+1 \in \mathbb{Z}$, $3 \nmid 3(n+1)$

Case 2: $x \equiv 0 (\text{mod } 4)$