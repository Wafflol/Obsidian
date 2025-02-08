$$T(n)=T\left( \frac{n}{2} \right)+10$$
$$=T\left( \frac{n}{4} \right)+20$$
$$=T\left( \frac{n}{8} \right)+30$$
$$T\left( \frac{n}{2^k} \right)+10k$$
$$\frac{n}{2^k}=10$$
$$k=\frac{\log_{2}n}{10}$$
$$T(n)=T\left( \frac{n}{n^{1/10}} \right)+\log_{2}n$$
A