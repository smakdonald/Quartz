#### $\thm$ – Solutions to Diophantine Equations
If $(x_{0}, y_{0})$ is a solution to the linear [[Diophantine Equation|Diophantine equation]] $ax + by = c$, then for all [[Integers|integers]] $t$, another solution is given by
$$x = x_0 - t  
\left( \frac{b}{\gcd(a, b)} 
\right)  \quad \quad \quad
y = y_{0} + t  
\left( \frac{a}{\gcd(a, b)} 
\right)  $$
Furthermore, these are all of the solutions.

##### *Proof.*
We leave to the reader the verification that if (x0, y0) is a solution, so is the  
(x, y) pair described in the theorem. To prove that this collection forms all solutions,  
suppose (x, y) is an arbitrary second solution, so that ax + by = c. Subtracting from this the equation ax0 + by0 = c and then dividing by g = \gcd(a, b) gives  
a  
g (x0 - x) = b  
g (y - y0).  
This last equality above shows that a  
g | b  
g (y - y0), and since a  
g and b  
g are relatively  
prime by Corollary 3.2.16, Euclid’s Lemma shows that a  
g | (y- y0). Writing y- y0 =  
t ( a  
g ) (which gives the desired parameterizaton of y), substitution into that last equality  
gives  
a  
g (x0 - x) = b  
g  
( ta  
g  
)  
,  
which provides  
x = x0 - t  
( b  
g  
)  
= x0 - t  
( b  
\gcd(a, b)  
)  
after multiplying by g  
a and then rearranging to solve for x.