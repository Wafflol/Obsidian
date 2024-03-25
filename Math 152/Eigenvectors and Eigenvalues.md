For an $n\times n$ transformation matrix $A$, a vector $\vec{v}$ and a scalar $\lambda$ are called an eigen-pair of $A$ for:
$$\vec{v} \neq 0$$
$$A\vec{v}=\lambda \vec{v}$$
$\vec{v}$ is the eigenvector, and $\lambda$ is the eigenvalue

Eigenvectors are never 0, but eigenvalues can be

For an $n\times n$ matrix, often there exist $n$ eigen-pairs, especially when no repeated eigenvalues occur

To calculate eigen-pairs:
We need to find a homogeneous solution for $A\vec{v}=\lambda \vec{v}$
$$(A-\lambda I)\vec{v}=0$$
$$\det(A-\lambda I) = 0$$
$$=\lambda^2-Tr\lambda+\det$$
Where Tr is the [[Trace|trace]]

Factoring this out:
$$(\lambda-\lambda_{1})(\lambda-\lambda_{2})=0$$
$$Tr = \lambda_{1}+\lambda_{2}$$
$$Det = \lambda_{1}\lambda_{2}$$

Thus, for any $2\times 2$ matrix, the [[Characteristic equation]] (polynomial) is:
$$\lambda^2-Tr\lambda+Det=0$$
