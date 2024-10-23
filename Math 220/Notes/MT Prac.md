Proof:



Scratch:
Rewrite:
$$\forall \epsilon > 0, \exists \delta > 0 \text{ } \text{ s.t. }(0 < \mid x-a \mid <\delta)\Rightarrow(\mid f(x)-L \mid )$$



$$\forall \epsilon > 0, \exists \delta > 0 \text{ } \text{ s.t. }(0 < \mid x-1 \mid <\delta)\Rightarrow\left( \mid f(x)- \left( \frac{1}{3} \right)\mid  \right) < \epsilon$$
$\mid f(x)-\frac{1}{3} \mid$
$$\frac{-2x+7}{3x+12}-\left( \frac{1}{3} \right) < \epsilon$$
$$\frac{-3x+3}{3x+12} < \epsilon$$
$$\mid\frac{-x+1}{x+4}\mid < \epsilon$$
$$|x-1 |< (\epsilon x+4\epsilon)$$
$$\mid x-1 \mid < \epsilon(x+4)$$

---

base case: $n = 7$
$$7! = 5040 > 3^7 = 2187$$
Inductive step:
Assume $n! > 3^n$
$$(n+1)! = (n+1)n!$$
Since $n! > 3^n$
$$(n+1)n! > 3^n (n+1)$$