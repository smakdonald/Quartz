#### $\cor$ – Units in Integer Rings
Let $d < 0$, and let $R$ be the ring of integers of $\Q[\sqrt{d}]$. Then with the exceptions 
of $d = -1$ and $d = -3$, we have $R^{\times} = \{\pm1\}$. 
For $d = -1$ we have $R^{\times} = \{\pm1, \pm i\}$, and for $d = -3$, $R^{\times} = \{\pm1,\pm \frac{1\pm\sqrt{-3}}{2}\}$.

##### *Proof.*
By Lemma 6.3.7, an element \mu \in\R is a unit if and only if it has norm \pm1, but 
norms of complex numbers are always positive, so we need only solve the equation 
N (\mu ) = +1. If d  \equiv 1 \mod 4, this is the equation 
1 = a^{2} - db^{2}. 
If d = -1, we quickly find the only solutions to be (a, b) = (\pm1, 0) and (a, b) = 
(0, \pm1), corresponding to the units \pm1 and \pmi respectively. When d < -1, the term 
-db^{2} is greater than 1 unless b = 0, so has no other solutions than (a, b) = (\pm1, 0), 
corresponding to the units \mu = \pm1. 
For the d \equiv 1 \mod 4 case, we need to solve the Diophantine equation 
1 = a^{2} + ab + b^{2} 
( 1 - d 
4 
) 
, 
or after a little algebra, the equivalent equation 
(2a + b)2 - db^{2} = 4. 
Again, both (2a + b)2 and -db^{2} are positive. If b = 0, then a = \pm1 and we retrieve 
the units \mu = \pm1 for any d. Now we look for any extra solutions: if d = -3, we 
find (a, b) = (0, \pm1), \pm(1, -1) corresponding to the units 
\mu = \pm 
( 
1 
2 \pm 
√-3 
2 
) 
, 
But for any other d \equiv 1 \mod 4, d is at most -7, and so -db^{2} > 4 whenever b  = 0, 
providing no more solutions.