#### $\thm$ – Universal Mapping Property for Quotient Rings
If $f: R \to S$ is a [[Ring|ring]] [[Homomorphism|homomorphism]] and $I \subseteq R$ is an [[Ideal|ideal]] such that $I \subseteq \ker(f)$[^1], there exists a well defined ring homomorphism $\overline{f}: R/I \to S$ such that $\overline{f} (r+I) = f(r)$. Furthermore, if $f$ is surjective then $\overline{f}$  is surjective and if $I=\ker(f)$ then $\overline{f}$ is injective.

###### *Proof.* 
Ignoring $\cdot$ for a minute, we know that there is a unique homomorphism $\overline{f}$ of abelian groups from $(R/I, +)$ to $(S, +)$ such that $\overline{f} (r+I) = f(r)$. It remains only to check that $\overline{f}$ preserves multiplication: Given elements $r + I, s + I \in R/I$, their product is $rs + I$, and we have
$$
\overline{f}(rs + I) = f(rs) = f(r)f(s) = f(r + I) f(s +I),
$$
since $f$ preserves multiplication.
***

[^1]: See: [[Kernel]]