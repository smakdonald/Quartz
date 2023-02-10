#### $\lem$ – Domains, Degrees, and Units
Assume $R$ is an [[Integral Domain|integral domain]].
1. $R[x_1, \dots, x_n]$[^1] is also an integral domain, for all $n \geq 1$.
2. $\deg(f g) = \deg(f) + \deg(g)$[^2] if $f$ and $g$ are nonzero polynomials of $R[x_1, \dots, x_n]$.
3. The [[Unit|units]] of $R[x_1, \dots, x_n]$ are $R[x_1, \dots, x_n]^\times=R^\times$[^3] (the invertible constants).

###### *Proof.* 
For (1), by induction checking the case $n=1$ is enough. For that case, just look at the leading terms in a product.

For (2), just look at the leading terms.

For (3), by induction it suffices to consider the case $n=1$. In that case, using (2) and the fact that $\deg(1) = 0$, we see than a unit in
$R[x]$ must have degree $0$, and then it's clear.
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Polynomial Degree]]
[^3]: See: [[Group of Units]]