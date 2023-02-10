#### $\thm$ – Properties of Splitting Fields
Let $F$ be a [[Field|field]] and $f(x) \in F[x]$[^1] a non-constant polynomial.
1. There exists a [[Splitting Field|splitting field]] $L$ for $f(x)$ over $F$.
2. If $F \subseteq L'$ is another splitting field of $f(x)$ over $F$, then there is a field [[Isomorphism|isomorphism]] $\s: L \xra{\cong} L'$ such that $\s|_F = \id_F$.
3. The [[Degree of Field Extension|degree]] of any splitting field of $f(x)$ is at most $n!$ where $n = \deg(f)$[^2]. 

##### *Proof.*
For (1), let $\ov{F}$ be an algebraic closure of $F$, which exists by the previous Theorem.  Let $\a_1, \dots, \a_m$ be the roots of $f(x)$ in $\ov{F}$, and set $L = F(\a_1, \dots, \a_m)$.

It is clear $L$ is a splitting field.

To prove (2), we proceed by induction on the degree of $f(x)$. If $f$ is linear, then the only splitting field of $f$ over $F$ is $F$ itself and so the result is clear in this case. Say $\a_1, \dots, \a_m$ and $\a'_1, \dots, \a'_m$ are the roots of $f(x)$ in $L$ and $L'$, respectively, and say they are ordered so that, $\a_m$ and $\a'_m$ are roots of the same irreducible factor of $f(x)$ in $F[x]$. 

By Corollary \ref{cor410} there is an isomorphism $\phi: F(\a_n) \xra{\cong} F(\a_n')$ that fixes $F$. Note that $f(x)$ factors as $(x-\a_n) g(x)$ in $F(\a_n)[x]$ and that $L$ is the splitting field of $g(x)$ over $F(\a_n)$, and similarly $f(x)$ factors as $(x-\a'_n) g'(x)$ in $F(\a'_n)[x]$ and that $L$ is the splitting field of $g'(x)$ over $F(\a'_n)$. If we blur our eyes slightly and pretend $\phi$ is the identity map, we can apply the inductive hypothesis, since $\deg(g) < \deg(f)$, to conclude that there is an isomorphism $\s$ as in the statement. I leave a more rigorous argument to your imaginations.

To prove (3), we also proceed by induction on the degree of $f$, using the same notation as in the proof of (2). 

Since $\a_n$ is a root of $f(x)$, we have $m_{F,\a_n} \mid f(x)$ and hence $$[F(\a_n): F] = \deg(m_{F,\a_n})  \leq n.$$ In $F(\a_n)$ we have $f(x) = (x-\a_n) g(x)$ with $g(x) \in F(\a_n)[x]$ and, as before, $L$ is  the splitting field of $g(x)$ over $F(\a_n)$, so that by induction $[L: F(\a_n)] \leq (n-1)!$.
By the degree formula $$[L: F] = [L: F(\a_n)][F(\a_n): F] \leq (n-1)! \cdot n = n!.$$
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Polynomial Degree]]