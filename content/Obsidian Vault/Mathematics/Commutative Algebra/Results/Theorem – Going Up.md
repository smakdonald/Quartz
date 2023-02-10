#### $\thm$ – Going Up
If $R \longrightarrow S$ is [[Integral Element|integral]], then for every $P \subsetneq P'$ in $\Spec(R)$[^1] and $Q \in \Spec(S)$ with $Q \cap R = P$[^2], there is some $Q' \in \Spec(S)$ with $Q \subsetneq Q'$ and $Q' \cap R = P'$.

##### *Proof.*
Consider the map $R / P \to S / Q$. This is integral, as we observed in \Cref{integral implies quotient integral}. It is also injective, so \hyperref[lying over]{Lying Over} applies. Thus, there is a prime $\aprime$ of $S/Q$ that contracts to the prime $P' / P$ in $\Spec(R/P)$. We can write $\aprime = Q' /  Q$ for some $Q' \in \Spec(S)$, and we must have that $Q'$ contracts to $P'$.

[^1]: Notation: [[Prime Spectrum]]
[^2]: Notation: [[Contraction]]