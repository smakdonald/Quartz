#### $\thm$ – Third Isomorphism Theorem
Suppose $G$ is a [[Group|group]], $M \leq N \leq G$[^1], $M \norm G$[^2] and $N \norm G$. Then $M \norm N$, $N/M \norm G/M$ and there is an [[Isomorphism|isomorphism]]
$$(G/M)/(N/M) \xra{\cong} G/N$$given by sending the [[Coset|coset]] of $(G/M)/(N/M)$[^3] represented by $gM$ to $gN$. 

###### *Proof.* 
The first two assertions are immediate from the definitions. #fix 

The [[Kernel|kernel]] of the canonical map $\can: G \onto G/N$ contains $M$ and so by the [[Theorem – UMP of a Quotient Group|UMP]] for quotients we get an induced [[Homomorphism|homomorphism]]
$$
\phi: G/M \to G/N
$$
with $\phi(gM) = \can(g) = gN$. Moreover, we know
$$
\ker(\phi) = \ker(\can)/M = N/M.
$$
Finally apply the [[Theorem – First Isomorphism Theorem|First Isomorphism Theorem]] to $\phi$.
***

[^1]: See: [[Subgroup]]
[^2]: See: [[Normal Subgroup]]
[^3]: See: [[Quotient Group]]

#### $\thm$ – Third Isomorphism Theorem for Rings
If $R$ is a [[Ring|ring]] and $I \subseteq J$ are two [[Ideal|ideals]] of $R$, then $J/I$[^4] is an ideal of $R/I$ and $$\frac{R/I}{J/I} \cong R/J \text{ via } (r + I) + J/I \mapsto r + J.$$

###### *Proof.* 
***
[^4]: See: [[Quotient Ring]]