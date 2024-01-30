#### When to use trig sub?
When you see:
$$
\sqrt{ a^2 - x^2 }, \sqrt{ a^2 + x^2 }, \sqrt{ x^2 - a^2 }
$$
Using the identities:
$$
1-\sin^2\theta = \cos^2\theta
$$
$$
1+\tan^2\theta = \sec^2\theta
$$
$$
\sec^2\theta-1 = \tan^2\theta
$$
multiply everything by $a^2$ and sub

$$
=a\cos \theta dx
$$
$$
x =a \sin \theta
$$
$$
dx = -a\sin^2\theta d\theta
$$
$$
\int  \, \sqrt{ a^2-a^2\sin^2\theta } a\cos \theta d\theta 
$$
$$
\int a^2 \cos^2\theta \, d\theta 
$$
$$
a^2\int \frac{1+\cos(2\theta)}{2} \, d\theta 
$$
$$
	=\frac{a^2}{2} \left( \theta +\frac{1}{2}\sin(2\theta) \right)) + C
$$

$$
=\frac{a^2}{2}(\theta + \sin \theta \cos \theta)+C
$$
$$
x = a\sin \theta \to \frac{x}{a} = \sin \theta
$$
Draw a triangle with hypotenuse $x$ and side $a$ 
close side = $\sqrt{ a^2 - x^2}$
opposite side = $x$
hypotenuse = $a$

Sub back in


Ex.

$$
\int \sqrt{ 3-2x-x^2 } \, dx 
$$
$$
\int \sqrt{ -(x^2+2x_-3) } \, dx 
$$
$$
\int \sqrt{ -(x^2+2x+1-4) } \, dx 
$$
$$
\int \sqrt{ -(x+1)^2 +4} \, dx 
$$
$$
\int \sqrt{ 4-(x+1)^2 } \, dx 
$$
let $x+1$ = $2\sin \theta$
$$
dx = 2\cos \theta d\theta
$$
$$
I = \int \sqrt{ 2^2-2^2\sin^2\theta }2\cos \theta \, d\theta 
$$
$$
=2^2\int \sqrt{ 1-\sin^2\theta }\cos \theta \, d\theta  
$$
$$
=4\int \cos ^2\theta \, d\theta 
$$
$$
 = 2(\theta+\sin \theta \cos \theta)+C
$$
We have $x+1 = 2\sin  \theta$, so $\arcsin\left( \frac{x+1}{2} \right) = \theta$
Now, $\sin\theta = \frac{x+1}{2}$
so $\cos \theta = \frac{\sqrt{ 2^2-(x+1)^2 }}{2}$
plug back in



Ex 2.
$$
\int \frac{1}{1-x^2} \, dx 
$$
Let $x = \sin \theta$, then $dx = \cos\theta d\theta$
So 
$$
\int \frac{1}{\sqrt{ 1-x^2 }} \, dx 
$$
$$
= \int \frac{1}{\sqrt{ 1-\sin^2\theta }}\cos\theta \, d\theta 
$$

#### Case 2:
For $\sqrt{ a^2 + x_2 }$
Let $x = a\tan\theta$, $dx = a\sec^2\theta d\theta$
$$
\sqrt{ a^2+x^2 } = \sqrt{ a^2+a^2\tan^2\theta } = a\sqrt{ 1+\tan^2\theta }
$$
$$
 = a\sqrt{ \sec^2\theta }
$$
$$
=a|\sec\theta|
$$
Since $\cos\theta >0$ for $\theta$ in $\left( -\frac{\pi}{2}, \frac{\pi}{2} \right)$, $\sec\theta = \frac{1}{\cos\theta} > 0$ also
So $a|\sec\theta| = a \sec\theta$

Ex.2 
$$
\int  \frac{1}{x^2+4x+7} \, dx
$$
$$
= \int \frac{1}{(x+2)^2+3} \, dx 
$$
$$
 = \int \frac{1}{(\sqrt{ 3 }^2+(2+x)^2)} \, dx 
$$
Let $x+2 = \sqrt{ 3 }\tan\theta$
$$
dx =\sqrt{ 3 }\sec^2\theta d\theta
$$
$$
I = \int \frac{1}{\sqrt{ 3 }^2+(\sqrt{ 3 }\tan\theta)^2}\sqrt{ 3 }\sec^2\theta \, d\theta 
$$
$$
= \frac{\sqrt{ 3 }}{3}\int \frac{\sec^2\theta}{1+\tan^2\theta} \, d\theta 
$$
$$
 = \frac{1}{\sqrt{ 3 }}\int 1 \, d\theta = \frac{1}{\sqrt{ 3 }}\theta+C 
$$
draw triangle and sub


#### Case 3:
For $\sqrt{ x^2 -a^{2}}$
Let $x = a\sec\theta$, $dx = a\sec\theta \tan\theta d\theta$

$$
\sqrt{ x^{2}-a^{2} } = \sqrt{ a^{2}\sec ^{2}\theta-a^{2} }
$$
$$
= a\sqrt{ \sec ^{2}\theta-1 }
$$
$$
a = \sqrt{ \tan^2\theta }
$$
$$
= a|\tan\theta|
$$
$$
=a\tan\theta \text{, since }\tan\theta >0 
$$

Ex.1
$$
I = \int \frac{1}{\sqrt{ x^{2}-16 }} \, dx 
$$
$$
=\int \frac{1}{\sqrt{ x^2-4^2 }} \, dx 
$$
$$
=\int \frac{1}{16\sec ^{2}\theta-16}4\tan\theta \sec\theta\, d\theta
$$
$$
=\int{ \frac{1}{\sqrt{ \sec ^{2}\theta-1 }}\tan\theta \sec\theta  }d\theta
$$
$$
= \int \sec\theta \, d\theta 
$$
$$
 = \ln|\sec\theta+\tan\theta|+C
$$
