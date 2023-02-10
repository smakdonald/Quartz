#### $\thm$ – Prime, Maximal, Domain, Field
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] with $1\neq 0$[^1], and let $I$ be an [[Ideal|ideal]] of $R$. 
1. The ideal $I$ is [[Mathematics/Modern Algebra/Definitions/Maximal Ideal|maximal]] if and only if $R/I$[^2] is a [[Field|field]]. 
2. The ideal $I$ is [[Mathematics/Modern Algebra/Definitions/Prime|prime]] if and only if $R/I$ is an [[Integral Domain|integral domain]]. 
3. Every maximal ideal of $R$ is prime.

###### *Proof.* 

The first assertion follows immediately from the Lattice Isomorphism Theorem and the fact that $R/I$ is a field if and only if its only ideals are $0$ and $R/I$.

Suppose $I$ is prime. If $(r + I)(r' + I) = 0 + I$, then $rr' \in I$ and hence either $r \in I$ or $r' \in I$, so that either $r + I = 0$ or $r'+ I  = 0$. This proves $R/I$ is a domain. Suppose $R/I$ is a domain and that $xy \in I$. Then $(x + I)(y + I) = 0$ in $R/I$ and hence either $x+ I = 0$ or $y + I = 0$. It follows $x \in I$ or $y \in I$, so that $I$ is prime.

If $I$ is maximal, then $R/I$ is a field, which in particular implies that $R/I$ is a domain, so $I$ is prime.
***

[^1]: See: [[Unital Ring]]
[^2]: See: [[Quotient Ring]]