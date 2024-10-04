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
Let $x = 0$
since $y \in  A$, $x+y = y$, and so it follows that $x+y \in A$. Thus, the implication is true.

d.
Proof by cases:

Case 1: $x+y \equiv 0 \text{(mod 3)}$
Let $z = 0$
$$\begin{align}
x+y &= 3n, n \in \mathbb{Z} \\
x+y+z &= 3n \\
&=3(n)
\end{align}$$
Since $n \in \mathbb{Z}$, it follows that $3 \mid n$ and thus, $3 \mid x+y+z$, so the implication is true in this case.

Case 2: $x+y \equiv 1 \text{(mod 3)}$
Let $z = 8$
$$\begin{align}
x + y &= 3n +1 \\
x + y + z & = 3n + 9 \\
&= 3(n+3)
\end{align}$$
Since $n+3 \in \mathbb{Z}$, it follows that $3 | n+3$ and thus, $3 | x+y+z$, so the implication is true in this case.

Case 3: $x+y \equiv 2 \text{(mod 3)}$
Let $z = 4$
$$\begin{align}
x + y &= 3n + 2 \\
x + y +z &= 3n + 6 \\
&= 3(n+2)
\end{align}$$
Since $n+2 \in \mathbb{Z}$, it follows that $3 \mid n + 3$, and thus, $3 \mid x +y+z$, so the implication is true in this case.

As the all cases are true, it follows that the implication is true in every case.

4.
a.
Negation: 
$$\exists n \in \mathbb{Z} \text{ } s.t. \text{ } \forall y \in \mathbb{R} - \{0\}, y^n>y$$

