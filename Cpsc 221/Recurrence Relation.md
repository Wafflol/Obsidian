$$T(n)=T\left( \frac{n}{2} \right)+5$$
$$=T\left( \frac{n}{4} \right)+10$$


$$=T\left( \frac{n}{8} \right)+15$$
$$=T\left( \frac{n}{2^k} \right)+5k$$
$$\frac{n}{2^k}=1$$
$$k = \log_{2}n$$
$$=T(1)+5(\log_{2}n)$$
$$=1+5\log_{2}n$$
---
$$T(n-1)+5$$
$$=T(n-2)+10$$
---
$$T(n)=2T\left( \frac{n}{2} \right)+5$$
$$=2\left( 2T\left( \frac{n}{4} \right)+5 \right)+5$$
$$=2^2T\left( \frac{n}{4} \right)+15$$
$$$$
$$2^2\left( 2T\left( \frac{n}{8} \right) +5\right)+15$$
$$= 2^3T\left( \frac{n}{2^3} \right)+35$$

$$5+5*2+5*4$$
$$=1, 3, 7, 15$$
$$5*(2^{k}-1)$$
$$=2^kT\left( \frac{n}{2^k} \right)+5*(2^{k}-1)$$
$$k = \log_{2}n$$
$$6n-5$$



