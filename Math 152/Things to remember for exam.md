1. Shortest distance from origin to line $L$:
	1. get a vector $\vec{v}$ from origin to point on $L$
	2. dist = $\begin{Vmatrix} \vec{v}-proj_{L}\vec{v}\end{Vmatrix}$ = $\begin{Vmatrix} \vec{v}-\vec{v}_{\perp}\end{Vmatrix}$ 
2. $\vec{a}\cdot \vec{b} = \begin{Vmatrix}a\end{Vmatrix}\begin{Vmatrix}b\end{Vmatrix}\cos\theta$
3. $Proj_{\vec{b}}\vec{a}=(\vec{a}\cdot \vec{b}) \frac{\vec{b}}{\begin{Vmatrix}\vec{b}\end{Vmatrix}^2}$
	1. $Proj_{\vec{u}}\vec{a}=(\vec{a}\cdot \vec{u})\vec{u}$
4. $$\vec{a}\cdot(\vec{b}\times \vec{c})=\begin{vmatrix}a_{1}&a_{2}&a_{3}\\b_{1}&b_{2}&b_{3}\\c_{1}&c_{2}&c_{3}\end{vmatrix}$$
5. $z = x+iy = \rho e^{i\theta}$ where $\rho = \sqrt{ x^2+y^2 }$ and $\theta$ = angle that the vector $\begin{bmatrix}x\\y\end{bmatrix}$ makes with $x_{1}$
6. $\begin{bmatrix}2 & 0 & 3 \\4 & 2 & 2 \\5 & 0 & 3\end{bmatrix}$ -> $\lambda_{1} = 2, \vec{v_{1}} = e_{2}$ 
7. in $\mathbb{R}^2$, $2M_{proj}-I = M_{\text{reflect}}$
8. in $\mathbb{R}^3$, for reflection and projection across plane, $M_{proj_{p}} = I-M_{proj_{\vec{n}}}, M_{Ref_{p}}=I - 2M_{proj_{p}}$