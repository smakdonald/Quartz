### Problem 6 – All Ideals Containing $(6, x^2 + x + 1)$
Find all the [[Ideal|ideals]] of $\Z[x]$ that contain $(6, x^2 + x + 1)$, the ideal of $\Z[x]$ [[Generator|generated]] by $6$ and  $x^2 + x + 1$. For each such ideal, give an explicit list of generators, and determine whether  
the ideal is [[Prime Ideal|prime]], [[Maximal Ideal|maximal]], or neither.

##### *Proof*.
First, notice that $x^2+x+1$ is [[Irreducible|irreducible]] in $\Z[x]$ as it is a cyclotomic polynomial. Thus the possibilities are the following:
- $I=(3,x^2+x+1)$,
- $J=(2,x^2+x+1)$,
- $L=(6,x^2+x+1)$, 
- $\Z[x]$.
Notice that $\Z[x]=(1)$, which is neither prime nor maximal, as those ideals must be proper. The ideal $L$ is not maximal as it is contained in both $I$ and $J$, nor is it prime, given that $3\cdot2\in L$ but neither $3$ nor $2$ are in $L$. 

Both $I$ and $J$ are generated with irreducible elements, making them irreducible ideals and thus maximal.
***
#qual