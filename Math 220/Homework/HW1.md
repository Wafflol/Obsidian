1.
$$n \in \mathbb{Z}$$
scratch
$$3 \nmid n^2+5n+5$$
$$\begin{align}
n^2+5n+5\neq 3k, k\in\mathbb{Z} \\

\end{align}$$
$$n^2+6n+5-n \neq 3k$$
$$(n+1)(n+5)-n\neq 3k$$
$$n+1\neq\frac{3k+n}{n+5}$$


---

$$3|n+1$$
$$n+1 = 3k, k\in\mathbb{Z}$$
$$n=3k-1$$
$$n^2+5n+5 = (3k-1)^2+5(3k-1)+5$$
$$=9k^2-6k+1+15k=9k^2+9k+1$$
$$=3(3k^2+3k)+1$$
the square & sum of integers are still integers, so $3k^2+3k \in \mathbb{Z}$
thus, $3|(3k^2+3k)$, but $3\nmid 3(3k^2+3k)+1$, as there will be a remainder of 1.
Thus, $$3 \nmid n^2+5n+5$$
Therefore, the implication is true

---
$$3\mid n+1$$
$$n+1 = 3k, k\in\mathbb{Z}$$
$$n = 3k-1$$
$$$$




2.
scratch
$$x^2-x-2<0$$
$$(x-2)(x+1)<0$$
$$\text{3 possible situations, x-2 is positive  and x+1 is positive, x-2 is negative and x+1 is positive, and both are negative}$$
to make a negative, you need a negative and positive
thus we have to choose when $\text{x-2 is negative and x+1 is positive}$
$x-2$ is negative when $x < 2$, and $x+1$ is positive when $x>-1$
thus, to make $(x-2)(x+1)$ negative, we need x to be between those numbers

proofs
$$\begin{align}

\end{align}$$
---
3.
let $x,y\in\mathbb{R}$
assume $x < y$, and $y^2< x^2$\
for $x^2 > y^2$, sqrt both sides so $\mid x \mid> \mid y\mid$
if both x and y are positive numbers, $\mid y\mid < \mid x\mid$ simplifies to $y<x$, which contradicts $x<y$
so x and y cannot both be positive, and at least one has to be negative. 
If $x$ is positive, it would contradict $\mid x\mid>\mid y\mid$, as $x<y$. Thus, we know $x$ has to be negative.
Consider two cases for $y$
Case 1:
if $y\geq 0$
since $\mid x\mid>\mid y\mid$ and $x<0$, $-x>y$
$x+y<0$.

Case 2:
$y<0$
the sum of two negative numbers is always negative. 
Thus, in this case, $x+y<0$
Therefore, as seen in these two cases, no matter the sign of $y$, $x+y<0$. Thus, the implication is true.
___
4.
$$n, a, b, x, y \in \mathbb{Z}$$
$$n \mid (ax+by)$$
$$ax+by=kn, k\in\mathbb{Z}$$
$$k = i+j,  i,j\in \mathbb{Z}$$
$$ax+by=in+jn$$
--
$$ax+by=0$$
$$ax=by$$
$$\frac{a}{y}=n \land \frac{b}{x} = n$$
$$a=yn \land b=xn$$
$$n\mid a \land n\mid b$$
fuckfuckfuckfuckfuckfuckfuckfuckfuckfuckf

---
Let $n, a, b, x, y \in \mathbb{Z}$
Assume $n \mid a$ and $n \mid b$
$$a = in \land b = jn \text{ for } i,j \in\mathbb{Z}$$
$$ax=ixn \land by = jyn$$
since $i, j, x, y \in \mathbb{Z}$, then it follows that $ix, jy \in \mathbb{Z}$
Thus, 
$$ax+by = ((ix)n+(jy)n)$$
$$ax+by=(ix+jy)n$$
because $ix,jy\in\mathbb{Z}$, $ix+jy \in\mathbb{Z}$
and thus, $n \mid (ax+by)$
Therefore, the implication is true.

---
5.
Prove $ab+cd$ is odd $(ab+cd) = 2k+1, k\in\mathbb{Z}$
Let $a, b, c, d, \in \mathbb{Z}$
Assume $a, c, b-d$ are odd
$$a = 2k+1, c = 2l+1, b-d=2m+1, \text{ }k, l, m \in \mathbb{Z}$$
$$b = 2m+1+d, d = b-2m-1$$
$$ab+cd = 4km+2k+2kd+2m+1+d+2lb+4lm-2l+b-2m-1$$
$$ab+cd=2(2km+k+kd+m+lb+2lm-l-m)+d+b$$
$(2km+k+kd+m+lb+2lm-l-m)\in\mathbb{Z}$, $o = (2km+k+kd+m+lb+2lm-l-m)$ so $o\in\mathbb{Z}$
$$ab+cd=2(o)+d+b$$
$$=2(o)+d+2m+1+d$$
$$=2(o + m + d)+1$$
since $(o + m + d)\in\mathbb{Z}$, $ab+cd$ is odd
Therefore, the implication is true.

---
6.
No.

Let $a \in \mathbb{Z}$ and assume that $3a+1$ is odd. Hence $3a+1=2k+1$ for some $k\in\mathbb{Z}$. This implies that $3a=2k$.
Since $k\in\mathbb{Z}$, $3a$ is even
Thus if we add $2a$+2, we get $$3a+2a+2$$
And since $a\in\mathbb{Z}$, $2a$ is even. 
Hence, $$2a = 2l, l\in\mathbb{Z}$$
$$3a+2a+2=5a+2=2k+2l+2$$
$$=2(k+l+1)$$
since $(k+l+1)\in\mathbb{Z}$, $5a+2$ is even
Therefore, the implication is true.

---
7.