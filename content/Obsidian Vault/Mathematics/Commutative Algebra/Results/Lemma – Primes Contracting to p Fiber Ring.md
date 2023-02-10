#### $\lem$ – Primes Contracting to p Fiber Ring
Let $\psi:R\to S$ be a ring homomorphism and $P \in \Spec(R)$[^1] be a [[Prime Ideal|prime ideal]]. The natural map $S \to \kappa_{\psi}(P)$ induces a homeomorphism (in particular, an order-preserving bijection)
$$\Spec( \kappa_{\psi}(P) ) \cong \{ Q \in \Spec(S) \ | \ \psi^*(Q) = P \},$$
where the right-hand side has the subspace topology induced by the [[Zariski Topology|Zariski topology]] on $\Spec(S)$.

##### *Proof.*
Consider the maps $$\begin{CD}
S@>\pi>>S/PS@>g>>(R\setminus P)\inv(S/PS).
\end{CD}$$For any localization map or any quotient map, the induced map on Spec is a homeomorphism onto its image. The map on spectra induced by $\pi$ can be identified with the inclusion of $V(P S)$ into $\Spec(S)$. For the second map, $g$, we saw in \Cref{localization ideals} that the map on spectra can be identified with the inclusion of the set of primes that do not intersect $R \setminus P$, i.e., those whose contraction is contained in $P$. Therefore, $(g \circ \pi)^*$ is injective, since it is the composition of two injective maps. 

On the one hand, if a prime $Q$ contains $PS$, then $Q \cap R \supseteq PS \cap R \supseteq P$. If moreover $Q \cap R \subseteq P$, we must have $Q \cap R = P$.

We have thus shown that the image of $(g \circ \pi)^*$ is the set of primes in $S$ that contract to $P$. %So $Q$ is in the image if and only if $\psi^{-1}(Q) = P$.

[^1]: Notation: [[Prime Spectrum]]