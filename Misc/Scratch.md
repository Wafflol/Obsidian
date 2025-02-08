$$T(n)=2\left( T\left( \frac{n}{2} \right) \right)+5$$
$$T(n)=4T\left( \frac{n}{4} \right)+15$$

$$T(n)=8T\left( \frac{n}{8} \right)+25$$
$$T(n)=2^kT\left( \frac{n}{2^k} \right)+5+10(k-1)$$
$$k=\log_{2}n$$
$$T(n)=n+5+10\log _{2}n-10$$
$$=n-5+10\log_{2}n$$