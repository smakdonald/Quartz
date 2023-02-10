### Problem 6 – Intersection of Splitting Fields
For [[Field|fields]] $E$ and $F$, we say $E$ is a *finite* [[Splitting Field|splitting field]] over $F$ if $E$ is the splitting field over $F$ of some polynomial $f(x)\in F [x]$[^1]. Assume $E$ and $K$ are both finite splitting fields over $\Q$ and prove $E \cap K$ is also a finite splitting field over $\Q$.

##### *Proof*.
Let $E$ and $K$ be finite splitting fields over $\Q$. So there exist polynomials $f,g\in F[x]$ such that $f$ splits in $F$ and $g$ splits in $E$. Note that both $E$ and $F$ are finite extensions, as each can be reached by adjoining each of the roots of $g$ and $f$, respectfully. 

If $E\cap F=\Q$ then we have our splitting field, as $\Q$ is a splitting field over itself.

Let $h$ be an irreducible polynomial in $F[x]$ with a root in $E\cap K$. Then $h$ has a root in $E$ and a root in $F$. If a splitting field has one root of a polynomial it has them all, and so we see that $h$ splits in both of these fields. Thus it splits in $E\cap K$. 
***
#qual

[^1]: Notation: [[Polynomial Ring]]