#### $\prop$ – Properties of Extension Degrees
Assume $F$ is a [[Field|field]] and $p(x) = \sum_i a_i x^i \in F[x]$[^1] is an [[Irreducible|irreducible]] polynomial. Set $L = F[x]/(p(x))$[^2], and for $f \in F[x]$, let $\ov{f}$ denote the [[Coset|coset]] $f(x) + (p(x)) \in L$. The following hold:
1. $F \into L$ is a field [[Field Extension|extension]] via the map given by $a \mapsto \ov{a}$ for $a \in F$. (This is technically an injective [[Homomorphism|homomorphisms]] of fields.)
2. $[L:F]=\deg(p)$.[^3]
3. $p(x)$ has a root in $L$; in fact, the element $\ov{x} \in L$ is a root of this polynomial: $\sum_i \ov{a_i} \cdot \ov{x}^i = 0 \in L$. 

##### *Proof.*
Because $p(x)$ is irreducible and $F[x]$ is a PID, $(p(x))$ is a maximal ideal. Thus $L = F[x]/(p(x))$ is a field. The map $F \to L$ given by $a \mapsto \ov{a}$ is a ring map since it is the composition of the two ring maps $F \xra{can} F[x] \xra{can} F[x]/(p(x))$. Since it is a ring map between two fields, it is injective. 

The equality $[L:F]=\deg(p)$ holds since $1, \ov{x}, \dots, \ov{x^{\deg(p)-1}}$ is a basis for $L$ regarded as an $F$-vector space, as we have seen before. 

The last assertion is tricky only because the notation is confusing. Say $p(x) = a_n x^n + \cdots + a_1 x + a_0$ and just to keep things straight let's set $q(y) = \ov{a_n} y^n  + \cdots + \ov{a_0} \in L[y]$. We need to show $q(\ov{x}) = 0$: We have
$$
q(\ov{x}) = \sum_i \ov{a_i} (\ov{x})^i =\sum_i \ov{a_i} (\ov{x^i}) = \ov{\sum_i a_i x_i}= \ov{p(x)}
= 0.
$$
***

[^1]: See: [[Polynomial Ring]]
[^2]: See: [[Principal Ideal]], [[Quotient Ring]]
[^3]: See: [[Degree of Field Extension]], [[Polynomial Degree]]