#### $\prop$ – Restriction of Scalars
Let $\phi: R \to S$ be a [[Ring|ring]] [[Homomorphism|homomorphism]]. Any left $S$-[[Module|module]] $M$ may be regarded via 'restriction of scalars' as a left $R$-module with the following structure:
- the rule for addition $+$ on $M$ is the same as in the original structure and
- the rule for scaling by elements of $R$ is
$$r \cdot m := \phi(r)m \text{ for any }r \in R \text{ and }m\in M.$$
###### *Proof.* 
Let $x,y \in R$ and $m,n \in M$. One checks that the properties in the definition of module hold for the given action using properties of ring homomorphisms. In detail, 
$$
(x+y)m =\phi(x + y)m= (\phi(x)+\phi(y))m=\phi(x)m + \phi(y)m=xm+ym,
$$
since $\phi$ preserves addition, 
$$
x(ym)=\phi(x) (\phi(y)m) = (\phi(x) \phi(y)) m = \phi(xy) m = (xy) m,
$$
since $\phi$ preserves multiplication,  and
$$
1 \cdot m = \phi(1) m = 1_S m = m
$$
since $\phi$ preserves multiplicative identities. This gives three of the axioms. The final also holds:
$$x(m + n) = \phi(x) (m+n) = \phi(x)m + \phi(x)n = xm + xn.$$
***