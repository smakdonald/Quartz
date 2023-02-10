#### $\lem$ – Image Criterion
Let $R \xrightarrow{\varphi} S$ be a ring homomorphism. For any $P \in \Spec(R)$[^1], $P \in \im(\varphi^*)$ if and only if[^2] 
$$P S \cap R = P.$$

##### *Proof.*
If $P S \cap R = P$, then 
$$\frac{R}{P} = \frac{R}{P S \cap R} \hookrightarrow \frac{S}{P S},$$
so localizing at $(R \setminus P)$, we get an inclusion $\kappa(P) \subseteq \kappa_{\varphi}(P)$. Since $\kappa(P)$ is nonzero, so is $\kappa_{\varphi}(P)$, and thus its spectrum is nonempty. By \Cref{lemma primes contracting to p fiber ring}, there is a prime mapping to $P$.

If $P S \cap R \neq P$, then $P S \cap R \supsetneq P$. If $Q \cap R = P$, then $Q \supseteq P S$, so $Q \cap R \supsetneq P$. So no prime contracts to $P$.

[^1]: Notation: [[Prime Spectrum]]
[^2]: Notation: [[Contraction]]