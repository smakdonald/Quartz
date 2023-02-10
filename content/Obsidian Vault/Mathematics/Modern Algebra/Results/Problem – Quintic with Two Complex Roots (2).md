### Problem 9 – Quintic with Two Complex Roots
Consider $f (x) = x^5-4x-2 \in \Q[x]$. This polynomial has exactly three real roots, a fact that you may use without proof.

(a) Show that $f$ is [[Irreducible|irreducible]] in $\Q[x]$.
(b) Let $L$ be a [[Splitting Field|splitting field]] of $f$ over $\Q$. Show that $L/\Q$ is a [[Galois Extension|Galois extension]] with [[Galois Extension|Galois group]] $\Gal(L/\Q)$ [[Isomorphism|isomorphic]] to the symmetric group $S_5$.

##### *Proof.*
Consider $f (x) = x^5-4x-2 \in \Q[x]$.

###### Part (a)
Using Eisenstein's Criterion with $p=2$ we see that $f$ is indeed irreducible in $\Q[x]$. 
***
###### Part (b)
Let $L$ be a splitting field of $f$ over $\Q$. As $f$ is monic and irreducible, it is the minimum polynomial for some $\a\in L$ such that $[\Q(\a):\Q]=5$. As $f$ has complex roots, we know that $\Q(\a)\neq L$, and is thus an intermediate field. By the FTGT there exists a subgroup $H$ of $\Gal(L/\Q)$ such that $H=\Gal(\Q(\a)/\Q)$. As $[\Q(\a):\Q]=5$ we know $|H|=5$, making $H=\langle\s\rangle$ for some $\s\in H$. Thus $\s$ is an element of order $5$ in $\Gal(L/\Q)$. As $f$ is a degree $5$ polynomial, we know $\Gal(L/\Q)$ is isomorphic to a subgroup of $S_5$. Thus $\s$ must be a $5$-cycle. 

Recall that $f$ has exactly two complex roots. Thus $\tau$, the complex conjugation automorphism, has order $2$, making it a transposition. From the Gospel of Mark we were told that we did not need to prove that a transposition and an $n$-cycle generate all of $S_n$, and thus $\Gal(L/\Q)\cong S_5$
***
#qual