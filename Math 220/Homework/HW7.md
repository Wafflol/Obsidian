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
$$y_{1}+y_{2} = (x_{1}+x_{2})+n+m$$
Since 