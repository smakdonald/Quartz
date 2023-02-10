### Problem 8 – Cubic Polynomial with Two Complex Roots
Let $F$ be the [[Splitting Field|splitting field]] over $\Q$ of the polynomial $x^3-2$. Prove that the [[Galois Extension|Galois group]] $\Gal(F : \Q)$ is [[Isomorphism|isomorphic]] to $S_3$.

###### *Proof*.
Let $F$ be the splitting field over $\Q$ of the polynomial $f(x)=x^3-2$, the roots of which are:
1. $\sqrt[3]2$
2. $\sqrt[3]2e^{2\pi i/3}$, and 
3. $\sqrt[3]2e^{4\pi i/3}$.
Using [[Theorem – Eisenstein's Criterion|Eisenstein's Criterion]] with $p=2$ we see that $f$ is [[Irreducible|irreducible]] in $\Q[x]$. As $f$ is monic and irreducible it is the [[Minimum Polynomial|minimum polynomial]] of $\sqrt[3]2\in\Q[x]$ and $[\Q(\sqrt[3]2):\Q]=3$. Thus, by the [[Theorem – Fundamental Theorem of Galois Theory|FTGT]] we know there exists an element of order $3$ in $\Gal(F:\Q)$. 

Notice now that  $f$ has exactly two complex roots, making complex conjugation correspond to a transposition in $S_3$. Thus we have an element of order $2$ and an element of order $3$, so the order of $\Gal(F:\Q)$ must be at least $6$ by [[Theorem – Lagrange's Theorem|Lagrange's Theorem]].

As $\deg f=3$ we know $\Gal(F:\Q)$ is isomorphic to a [[Subgroup|subgroup]] of $S_3$ (See: [[Proposition – Automorphisms and Permutations (Fields)|Proposition]]), which has order $6$. Thus $\Gal(F : \Q)$ is isomorphic to $S_3$.
***
#qual