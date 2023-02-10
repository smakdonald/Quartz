#### $\prop$ – Criteria for Separability
Let $F$ be [[Field|field]] and $\ov{F}$ an [[Algebraic Closure]] of $F$. 
1. Given $f(x) \in F[x]$[^2] and $\a \in \ov{F}$, the [[Multiplicity|multiplicity]] of $\a$ in $f(x)$ is at least $2$ if and only if $f(\a) = 0$ and $f'(\a) = 0$[^1].
2. $f$ is [[Separable|separable]] if and only if $\gcd(f(x), f'(x)) = 1$ in $F[x]$. 
3. If $f(x)$ is [[Irreducible|irreducible]] in $F[x]$, then $f$ is separable if and only if $f'(x) \neq 0$.

##### *Proof.*
For (1), suppose $\a$ is a root of $f(x)$ of multiplicity at least two. Then $f(x) = (x-\a)^2g(x)$ in $\ov{F}[x]$ and hence $f'(x) = 2(x - \a) g(x) + (x-\a)^2 g(x)$, by the Product Rule. It follows that $f'(\a) = 0$. Conversely, suppose $f(\a) = f'(\a) =0$. Since $f(\a) = 0$, we have $f(x) = (x-\a)h(x)$ and hence $f'(x) = h(x) + (x-\a)h'(x)$. Since $f'(\a) = 0$ it follows $h(\a) = 0$ and thus $\a$ has multiplicity at least two. 

For the second assertion, by (1), we have that $f$ is separable if and only if $f$ and $f'$ has no common roots in $\ov{F}$. The result thus follows from the Lemma.

For the final assertion, assume $f(x)$ is irreducible. Since the degree of $f'(x)$ is strictly less than the degree of $f(x)$, we have that $\gcd(f(x),f'(x)) \ne 1$ if and only if  $f'(x) = 0$.
***

[^1]: See: [[Derivative]]
[^2]: See: [[Polynomial Ring]]