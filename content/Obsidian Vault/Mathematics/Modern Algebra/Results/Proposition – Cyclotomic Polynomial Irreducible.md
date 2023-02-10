#### $\prop$ – Cyclotomic Polynomial Irreducible
For any prime $p$, the $p$-th *cyclotomic polynomial* $$f(x) = x^{p-1} + x^{p-2} + \cdots + x^2 + x+1 \in \Z[x]$$is [[Irreducible|irreducible]] in $\Q[x]$[^1].

##### *Proof.*
Consider the [[Ring|ring]] [[Isomorphism|isomorphism]] $\phi: \Q[x] \xra{\cong} \Q[y]$ given by $\phi(h(x)) = h(y+1)$. 
I claim that
$$
\phi(f(x)) = y^{p-1} + p y^{p-2} + {p \choose 2} y^{p-3} +{p \choose 3} y^{p-4} +
\cdots + {p \choose p-1} y + p.
$$
To see this, we note that $f(x) (x-1) = x^p - 1$ and by the binomial theorem we have $$\phi(x^p-1) = (y+1)^p - 1 = y^p + p y^{p-1} + {p \choose 2} y^{p-2} + \cdots + py.$$
Since $\phi(x^p-1) = \phi(f(x)) \phi(x-1) = \phi(f(x)) y$, the claim follows.

By [[Theorem – Eisenstein's Criterion|Eisenstein]], $\phi(f(x))$ is irreducible in $\Q[y]$ and, since $\phi$ is an isomorphism, it follows that $f(x)$ is irreducible in $\Q[x]$.
***

[^1]: See: [[Polynomial Ring]]