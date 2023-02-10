#### $\cor$ – Uniqueness of Field Extensions
Let $p(x)\in F[x]$ be [[Irreducible|irreducible]] and let $\a$ (respectively, $\a'$) be a root of $p(x)$ in some [[Ring|field]] [[Field Extension|extension]] $L$ (respectively, $L'$) of $F$. Then there is an [[Isomorphism|isomorphism]] of fields $\theta: F(\a) \xra{\cong} F(\a')$ such that $\theta|_F = \id_F$ and $\theta(\a) = \a'$.

##### *Proof.*
Note that $p(x)$ is (up to a non-zero constant factor) the minimum polynomial of both $\a$ and $\a'$.
So, we may apply (3b) of the Theorem twice to give a pair of isomorphisms $$F(\a) \xla{\cong} F[x]/(p(x)) \xra{\cong} F(\a').$$of fields, given by sending $\ov{f(x)}$ to $f(\a)$ (for the left one) and $f(\a')$ (for the right one). Take $\theta$ to be the inverse of the one on the left composed with the right one. 
***