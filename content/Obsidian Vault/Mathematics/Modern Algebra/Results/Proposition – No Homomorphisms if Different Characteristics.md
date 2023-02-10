#### $\prop$ – No Homomorphisms if Different Characteristics
If $F$ and $E$ are [[Field|fields]] such that $\char(F) \ne \char(E)$[^1] then there exist no [[Ring|ring]] [[Homomorphism|homomorphisms]] from $E$ to $F$ (or vice versa).

##### *Proof.*
Suppose $F$ and $E$ are fields and $\s: F \to E$ is a ring homomorphism. Let $\phi_F: \Z \to F$ and $\phi_E: \Z \to E$ be the unique ring maps from $\Z$ to $F$ and $E$. Since $\s \circ \phi_F$ is a ring map from $\Z$ to $E$, we have $\s \circ \phi_F = \phi_E$ by the uniqueness of $\phi_E$. Since $F$ is a field and $E$ is not the zero ring, the map $\s$ is injective. Since $\s$ is injective, it follows that $\ker(\s \circ \phi_F) = \ker(\phi_F)$, and hence we obtain that $\ker(\phi_F) = \ker(\phi_E)$. By definition of characteristic, we conclude $\ker(E) = \ker(F)$.
***

[^1]: See: [[Mathematics/Modern Algebra/Definitions/Ring Characteristic]]