#### $\prop$ – Primes and Irreducibility
Assume $R$ is an [[Integral Domain|integral domain]] and $f(x) \in R[x]$[^1] is a monic polynomial with coefficients in $R$. If there is a [[Mathematics/Modern Algebra/Definitions/Prime|prime]] element $p \in R$ such that $\ov{f} \in (R/p)[x]$ is [[Irreducible]] in $(R/p)[x]$, then $f$ is irreducible in $R[x]$.

##### *Proof.*
We prove the contra-positive. Suppose $f$ is reducible in $R[x]$. Then we have $f(x) = g(x) h(x)$ for some monic, non-constant polynomials $g$ and $h$ in $R[x]$. It follows that $\ov{f} = \ov{gh} = \ov{g} \ov{h}$ holds in $(R/p)[x]$. But since $g$ and $h$ are monic, non-constant polynomials, $\ov{g}$ and $\ov{h}$ are both non-constant polynomials in $(R/p)[x]$ and hence $\ov{f}$ is reducible in $(R/p)[x]$.
***

[^1]: See: [[Polynomial Ring]]