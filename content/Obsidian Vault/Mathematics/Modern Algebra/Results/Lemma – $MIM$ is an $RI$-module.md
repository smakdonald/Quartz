#### $\lem$ – $M/IM$ is an $R/I$-module
For a commutative [[Ring|ring]] $R$, [[Module|module]] $M$ and [[Ideal|ideal]] $I$, the rules for addition in $M/IM$[^1] and scaling by $R/I$ on $M/IM$ introduced above make $M/IM$ into an $R/I$-module.

Moreover, given another $R$-module $N$ and an $R$-map $f: M \to N$, the function $\ov{f}: M/IM \to N/IN$ given by $\ov{f}(m + IM) = f(m) + IN$ is a well-defined $R/I$-module [[Homomorphism|homomorphism]].

Finally, if $g: N \to P$ is yet another $R$-module homomorphism, then $\ov{g} \circ \ov{f} = \ov{g \circ f}$, and we also have $\ov{\id_M} = \id_{M/IM}$ for any $R$-module $M$.

###### *Proof.* 
I leave some of the details as an exercise, but I will check a few of the necessary things:

We already showed that the rule for scaling is well defined, and we know from 817 that the rule for addition is well-defined and that $(M/IM, +)$ is an abelian group. To show $M/IM$ is an $R/I$-module, there remain four axioms to verify. For instance, $((r+I)(s+I))(m +IM) = (rs + I)(m + IM) = (rsm + IM) = (r+I)(sm +IM) = (r+I)((s+I)(m+IM))$, which verifies one of them; the other proofs are similar. 

Next, let me verify that  the function $\ov{f}$ is a well-defined $R/I$-map: Let $g: M \to N/IN$ be the composition of $R$-maps $M \xra{f} N \to N/IN$ (the second one being the canonical one), so that $g(m) = f(m) + IN$. Since $f(\sum_i a_i m_i) = \sum a_i f(m_i) \in IN$ for any $a_i$'s belonging to $I$ and  $m_i$'s belonging to $M$, we have $IM \subseteq \ker(g)$. By the UMP for quotient modules, there is an induced $R$-map $\ov{f}: M/IM \to N/IN$ given by $\ov{f}(m + IM) = f(m) + IN$. The map $\ov{f}$ is so far only known to be an $R$-map, but it is in fact an $R/I$-map since$$\ov{f}((r + I)(m +IM)) =   \ov{f}(rm +IM) = f(rm) + IN = rf(m) + IN = (r+I)(f(m) + IN).$$The final assertions are clear from the formula for $\ov{f}$ for an $R$-map $f$. 
***

[^1]: See: #fix 