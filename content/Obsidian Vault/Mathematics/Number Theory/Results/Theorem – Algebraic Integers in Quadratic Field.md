#### $\thm$ – Algebraic Integers in Quadratic Field
Let $d\neq 0$, 1 be a square-free integer. Then: 
• If $d\not\equiv 1 \mod 4$, then the [[Ring of Integers|ring of integers]] of $\Q[\sqrt{d}]$ is 
$$\Z[\sqrt{d}] = {a + b\sqrt{d} : a, b \in\Z}$$
• If $d \equiv 1 \mod 4$, then the ring of integers of $\Q[\sqrt{d}]$ is 
$$\Z \left[\frac{1+\sqrt{d}}{2}\right]\left\{ 
a + b \left(\frac{1+\sqrt{d}}{2}\right): a, b \in\Z\right\}$$
##### *Proof.*
182 6 Number Theory, from Where We R to Across the C 
Definition 6.3.4 
The ring of integers of a quadratic field is the subset of elements of the field that 
are algebraic integers.  
Of course, you can’t define a set into being a ring. That these sets are rings is a small 
part of the following theorem, which gives an explicit description of the algebraic 
integers of a quadratic field. 
Theorem 6.3.5 
Let d  = 0, 1 be a square-free integer. Then: 
• If d  \equiv 1 (\mod 4), then the ring of integers of Q[\sqrt{d}] is 
Z[\sqrt{d}] = {a + b\sqrt{d} : a, b \in\Z} 
• If d \equiv 1 (\mod 4), then the ring of integers of Q[\sqrt{d}] is 
Z 
[ 
1 + \sqrt{d} 
2 
] 
{ 
a + b 
( 1+\sqrt{d} 
2 
) 
: a, b \in\Z 
} 
Proof First, it is routine to verify that the described numbers are algebraic integers in 
both cases: the quadratic formula verifies that the number a + b\sqrt{d} has the minimal 
polynomial 
(x - (a + b\sqrt{d}))(x - (a - b\sqrt{d})) = x^{2} - 2ax + (a^{2} - db^{2}) \in\Z[x], 
and the number a + b 
( 1+\sqrt{d} 
2 
) 
has minimal polynomial 
x^{2} - (2a + b)x + a^{2} + ab - b^{2} 
( d - 1 
4 
) 
, 
which is in Z[x] since d \equiv 1 \mod 4. 
It remains to show the reverse direction, that if \a \in\Q[\sqrt{d}] is an algebraic integer 
then it is in Z[ 1+\sqrt{d} 
2 ] when d \equiv 1 (\mod 4) and is in Z[\sqrt{d}] otherwise. 
Suppose \a = a+b\sqrt{d} \in\Q[\sqrt{d}] is an algebraic integer, so its minimal polynomial 
x^{2} - 2ax + (a^{2} - db^{2}) has integer coefficients. Let e = 2a and f = a^{2} - db^{2}. Write 
b = m 
n for m, n \in\Z with \gcd(m, n) = 1. Then substituting a = e 
2 and b = m 
n into 
the expression for f and clearing denominators gives 
e2n2 - 4dm2 = 4 f n2.
This shows that e2n2 must be a multiple of 4, and so at least one of e or n is even. 
We break into these two cases. 
First, if e is even, then a = e 
2 is an integer, and hence a^{2} - f = db^{2} = dm2 
n2 must 
be an integer as well, so n2 | dm2. Since \gcd(m, n) = 1, Euclid’s Lemma shows that 
n2 | d, which since d is square-free implies that n = \pm1. Since b = m 
n, this shows 
that b, along with a, must be an integer. 
Otherwise e is odd and n is even, and since \gcd(m, n) = 1, m must be odd. 
Substituting n = 2t into (∗) and canceling a factor of 4 gives 
e2t2 - dm2 = 4 f t2. 
Since e and m are odd, we have e2 \equiv m2 \equiv 1 \mod 4 and so reducing this equation 
\mod 4 gives t2 \equiv d \mod 4. Since d is a square \mod 4, d is either 0 or 1 \mod 4, 
but since d is square-free, we know 4  d and hence d \equiv 1 \mod 4. Substituting 
m = nb = 2tb into e2t2 - dm2 = 4 f t2, we find e2t2 - d(2tb)2 = 4 f t2, so we see 
that t2 | d(2tb)2. Say d(2tb)2 = t2k. (We stress that b is not necessarily an integer, 
but 2tb is.) 
Since d is square-free, it must be the case that t2 | (2tb)2, and so (2b)2 \in\Z. It 
thus makes sense to cancel a t2 and reduce \mod 4: 
e2t2 - d(2tb)2 = 4 f t2 
e2 - d(2b)2 = 4 f 
1 - 1(2b)2 \equiv 0 \mod 4, 
showing that 2b must be odd. 
Combining the two cases, we conclude that for a + b\sqrt{d} (a, b \in\Q) to be an 
algebraic integer we must either have a and b both integers, or 2a and 2b both odd 
integers and d \equiv 1 \mod 4. That is, if d  \equiv 1 (\mod 4), then a + b\sqrt{d} is an algebraic 
integer if and only if a, b \in\Z. If d \equiv 1 (\mod 4), then those same numbers are 
algebraic integers, and so are the a + b\sqrt{d} for which a and b are both half-integers. 
Finally, given our explicit descriptions of these sets, it is easy to verify that they 
are rings. The only ring axioms that need checking are that the two sets are closed 
under addition and multiplication. Of these, addition is trivial and multiplication 
follows from the identities 
(a + b\sqrt{d})(m + n\sqrt{d}) = (am + bdn) + (an + bm)\sqrt{d} \in\Z[\sqrt{d}] 
and, writing \g = 1+\sqrt{d} 
2 when d \equiv 1 \mod 4, 
(a + b\g ) (m + n\g ) = 
( 
am + bn \cdot d - 1 
4 
) 
+ (an + bn + bm)\g \in\Z 
[ 
1 + \sqrt{d} 
2 
] 
, 
both verifiable via direct computation.