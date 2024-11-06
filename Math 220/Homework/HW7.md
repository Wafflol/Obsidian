1.
To begin, the power set $\mathcal{P}(\{ 1, 2 \})$ is: 
$$\{ \emptyset, \{ 1 \}, \{ 2 \}, \{ 1, 2 \} \}$$
Thus, using the definition of the relation $\mathcal{R}$, the elements in $\mathcal{R}$ are: 
$$\mathcal{R} = \{ (\emptyset, \emptyset), (\emptyset, \{ 1 \}), (\{ 1 \}, \emptyset), (\emptyset, \{ 2 \}), (\{ 2 \}, \emptyset) , (\emptyset, \{ 1, 2 \}), (\{ 1, 2 \}, \emptyset) , (\{ 1 \}, \{ 2 \}), (\{ 2 \}, \{ 1 \})\}$$

2.1
Let $R$ be reflexive. Then, as the definition of reflexivity states that a relation $R$ is reflexive when $\forall b \in B, a R a$, it follows that $\forall a \in A$, if $R$ is reflexive, then $(a, a) \in R$, and thus, as $\bar{R} = (A \times A) - R$, then it follows that $(a, a) \not\in \bar{R}$ .
Thus, it follows that $\bar{R}$ is not reflexive, and the implication is false.

2.2
Let $R$ be symmetric. Then, as the definition of symmetry states that a relation $\mathcal{R}$ is symmetric when $\forall a, b,  a R b \Rightarrow b Ra$, it follows that $\forall a,b \in A$, if $R$ is symmetric, then $(a, b), (b, a) \in R$, and thus, as $\bar{R} = (A \times A) - R$, then it follows that $(a, b), (b, a) \not\in \bar{R}$ .
Thus, it follows that $\bar{R}$ is not symmetric, and the implication is false.

2.3
Let $R$ be transitive. Then, as the definition of transitivity states that a relation $R$ is transitive when $\forall a, b, c, (a Rb) \land (bRc) \Rightarrow a Rc$, so because $(a, b), (b,c) \in R$, and $\bar{R} = (A \times A) - R$, then it follows that $(a, b), (b, c) \not\in R$. Thus, it follows that the implication is false.

3.
The implication states: $(aRc \land b Rc) \Rightarrow aRb$.
Let $c = a$, so that the implication becomes $(aRa \land bRa) \Rightarrow aRb$
Since we know $aRa$, as $R$ is reflexive, $aRa$ is always true, and using the identity law, we can eliminate the $aRa$ term, leaving us with $bRa \Rightarrow aRb$, and so it follows that $R$ is symmetric.
Since we know $R$ is symmetric, we can flip the second term to get:
$$(aRc \land cRb) \Rightarrow aRb$$
Thus, it follows that $R$ is transitive, and thus, the implication is true.

4.
layman -> x,y -> x < y + 1
a.
Using the relation $\mathcal{R}$, since $x_{1}Ry_{1}$ and $x_{2} R y_{2}$, it follows that: 
$$y_{1}=x_{1}+ n, y_{2} = x_{2} + m, \text{ where }n,m \in \mathbb{N}$$
Thus, it follows that
$$\begin{align}
y_{1}+y_{2} &= (x_{1}+x_{2})+n+m \\
\end{align}$$
Since $x_{1}+x_{2} \in \mathbb{R}$, and $m+n \in \mathbb{N}$, then it follows that $(x_{1}+x_{2}) \mathcal{R} (y_{1}+y_{2})$. Thus, the implication is true.

b.
Using the relation $\mathcal{R}$, since $x_{1}Ry_{1} \text{ and } x_{2} R y_{2}$, it follows that:
$$y_{1} = x_{1}+n, y_{2}=x_{2} + m, \text{ where } n, m, \in \mathbb{N}$$
Thus, it follows that 
$$x_{1}y_{1} = x_{1}^2+x_{1}n, x_{2}y_{2} = x_{2}^2+x_{2}m$$
Let $x_{2} = 1, m = 2, x_{1} = 2, n = 3$
$$\begin{align}
x_{2}y_{2} &= 1+2=3 \\
x_{1}y_{1} &= 4+6=10
\end{align}$$
By the definition of the relation, since $x_{1}y_{1} = 10$ and $x_{2}y_{2} = 3$, $x_{1}y_{1}>x_{2}y_{2}$, and since the relation $x_{1}y_{1}Rx_{2}y_{2}$ states that $x_{2}y_{2}=x_{1}y_{1}+l, l \in \mathbb{N}$, the relation is not true, as $l$ is always positive and as already stated, $x_{1}y_{1}>x_{2}y_{2}$. Thus, it follows that $x_{1}y_{1} \bar{R} x_{2}y_{2}$, and thus the implication is false.

5.
Reflexive:
First take the reverse of the relation:
$$\frac{a}{b} \in \mathbb{Q} \iff aTb$$
Assume $\frac{a}{b} \in \mathbb{Q}$
Let $b = a$, then $\frac{a}{a} \in \mathbb{Q}$
and since we know the domain of the relation is $\mathbb{R} - {0}$, $a \neq 0$, and thus, $\frac{a}{a} = 1 \in Q$. Thus, as $\frac{a}{a} \in Q$, it follows that $aTa$.

Symmetric:
Again, starting with the reverse:
$$\frac{a}{b} \in \mathbb{Q} \iff aTb$$
Assume $\frac{a}{b} \in \mathbb{Q}$
By the definition of rationality, that means that $\frac{a}{b} = \frac{c}{d}$, where $c, d, \in \mathbb{Z}$, and thus, 
$\frac{d}{c} \in \mathbb{Q}$, and it follows that $\frac{b}{a} \in \mathbb{Q}$
Thus, it follows that 
$$\begin{align}
\frac{a}{b} \in \mathbb{Q} \Rightarrow aTb \\
\frac{b}{a} \in \mathbb{Q} \Rightarrow bTa
\end{align}$$
and thus, since $aTb$ and $bTa$, it follows that $T$ is symmetric.

Transitive:
Again, starting with the reverse:
$$\frac{a}{b} \in \mathbb{Q} \iff aTb$$
Assume $\frac{a}{b} \in \mathbb{Q}$, and let $\frac{b}{c} \in \mathbb{Q}$
Then:
$$\begin{align}
\frac{a}{b} \in \mathbb{Q} \Rightarrow aTb \\
\frac{b}{c} \in \mathbb{Q} \Rightarrow bTc
\end{align}$$
Since $\frac{a}{b}, \frac{b}{c} \in \mathbb{Q}$, $\frac{a}{b} = \frac{d}{e}, \frac{b}{c} = \frac{f}{g}, d,e,f,g \in \mathbb{Z}$
Thus, 
$$\begin{align}
\frac{ae}{d}=b&, b=\frac{cf}{g} \\
\frac{ae}{d} &= \frac{cf}{g} \\
\frac{a}{c} &= \frac{fd}{eg}
\end{align}$$
Since $fd, eg \in \mathbb{Z}$, then $\frac{fd}{eg} \in \mathbb{Q}$, and thus $\frac{a}{c} \in \mathbb{Q}$, so it follows that $aTc$. Thus, the implication is true, a $aTb, bTc$, and $aTc$.

6.
