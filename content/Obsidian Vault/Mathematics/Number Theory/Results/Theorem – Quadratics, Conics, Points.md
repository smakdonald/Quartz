#### $\thm$ – Quadratics, Conics, Points
Let $p$ be an odd prime, and $f (x) = x^{2} + sx + t$ a quadratic polynomial over 
$\Z/( p)$ with non-zero discriminant $(s^{2} - 4t  = 0)$. Then the conic $y^{2} = f (x)$ 
has precisely $p - 1$ points on it.

##### *Proof.*
7.4 Application: Counting Points on Curves 219 
Proof First, since p is odd, 2 is invertible modulo p, so we can “complete the square” 
to re-write the conic as 
y^{2} = x^{2} + sx + t = 
 
x + s 
2 
2 
+ u 
where u = t - s2 
4 = 4t-s2 
4  = 0 by the discriminant hypothesis. (Note that we are 
writing s 
2 as a shorthand for s \cdot 2-1 ). Rearranging gives 
u = y^{2} - 
 
x + s 
2 
 
y - x - s 
2 
  
y + x + s 
2 
 
. 
Thus every point on the conic provides a factorization of u in \Z/( p). Conversely, 
given a factorization u = u1u2, then the system 
u1 = y - x - s 
2 
u2 = y + x + s 
2 
provides the following solution to the conic: 
x = u2 - u1 - s 
2 y = u1 + u2 
2. 
We thus have a bijection between points on the conic and (ordered) factorizations of 
u into two factors u = u1u2 in \Z/( p). This establishes the result, as there are exactly 
p - 1 such factorizations: for any u1  = 0 in \Z/( p), there is a unique u2, namely 
u2 = uu-1 
1, that gives a factorization.