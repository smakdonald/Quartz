#### $\thm$ – Inverses in $\Z/(n)$
The element $[a] \in\Z/(n)$[^1] has a multiplicative inverse if and only if $\gcd(a, n)=1$[^2]

##### *Proof.*
By Bézout’s Identity, if \gcd(a, n) = 1, there exist x and y so that ax +ny = 1,  
and reducing this equation \mod n gives ax \equiv 1 (\mod n). That is, [x] = [a]-1  
provides a multiplicative inverse. Conversely, if ax \equiv 1 (\mod n), then by definition  
of modular congruence n | 1 - ax, and so 1 - ax = ny for some y \in\Z, giving  
ax + ny = 1. Thus by the Fundamental Theorem of \gcds, \gcd(a, n) = 1.

[^1]: Notation: [[Equivalence Class]], [[Z(n)]]
[^2]: Notation: [[GCD]]