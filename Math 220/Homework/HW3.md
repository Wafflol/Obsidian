1.
$$\exists c \in \mathbb{R} \text{ } s.t. \forall \epsilon >0,\exists M >0 s.t. \text{when } x\geq M,\left|\frac{x^2+\sin(x^2)}{x^2+\cos(x)} -c \right| < \epsilon $$
the negation:
$$\forall c \in \mathbb{R}, \exists \epsilon > 0 s.t. \forall M > 0, \text{ when } x\geq M, \left | \frac{x^2+\sin(x^2)}{x^2+\cos(x)}-c\right| \geq \epsilon$$

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
Proving the original statement:
Let $n \in \mathbb{Z}$
Let $y = 1$
When $n = 0$, $1^0 = 1$, and since 1 to the power of anything else is still $= 1$, the implication is true.

b.
Negation:
$$\forall y \in \mathbb{R}- \{0\}, \exists n \in \mathbb{Z} \text{ } s.t. \text{ } y^n > y$$
Proving the original statement:
Let $y = 1$
Case 1: $n = 0$
$$\begin{align}
y^n = 1^0 = 1
\end{align}$$

Case 2: $n \neq 0$
$$\begin{align}
y^n = 1^n = 1
\end{align}$$

Since in both of these cases, $y^n = y$, it follows that the implication is true.

c.
Negation: 
$$\exists x \in \mathbb{R} \text{ where  } x \neq 0 \text{ }s.t. \text{ }  (x > 1 )\land ( \frac{1}{x} > 1)$$
Prove original statement:
Proof by cases:

Case 1: $x < 0$
Since $x < 0$, and $0 <1$, then the implication is true in this case.

Case 2: $0< x< 1$
Similarly to case 1, since $x < 1$, the implication is true in this case.

Case 3: $x \geq 1$
Since $x \neq 0$, we can divide by x if we need to
$$x \geq 1$$
dividing both sides by x:
$$1 \geq \frac{1}{x}$$

Thus, in all cases, the implication holds true.

d.
Negation: 
$$\exists x \in \mathbb{R} \text{ where } x \neq 0 \text{ } s.t. ( x < 1) \land (\frac{1}{x} < 1)$$
Prove original statement:
When $x = -2$:
$$ \frac{1}{x} = -\frac{1}{2}  < 1$$
$$x = -2 < 1$$
Thus, it follows that the negation is true. Since the negation is true, the original statement is false.

5.
a.
Reformulated statement: $$\exists k \in K \text{ } s.t. \text{ } \exists l \in L \text{ } s.t. \text{ } k \text{ unlocks } l$$
Negation:
$$\forall k \in K, \forall l \in L, k \text{ does not unlock } l$$
Reformulated negation: All of the keys do not unlock all of the locks

b.
Reformulated statement:
$$\exists k \in K \text{ } s.t. \forall l \in L\text{, } k \text{ unlocks } l$$
Negation: 
$$\text{ } \forall k \in K, \exists l \in L \text{ } s.t. \text{ } k \text{ does not unlock } l$$
Reformulated negation: All keys do not unlock some lock

c.
Reformulated statement:
$$\exists l \in L \text{ } s.t. \text{ } \forall k \in K, k \text{ does not unlock }l$$
Negation:
$$\forall l \in L, \exists k \in K \text{ } s.t. \text{ } k \text{ unlocks } l$$
Reformulated negation: All locks can be unlocked by some key
