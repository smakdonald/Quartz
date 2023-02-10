#### $\cor$ – Finite Contractions in Int Noeth Alg
Let $S$ be an [[Integral Element|integral]] $R$-[[Algebra|algebra]]. If $S$ is [[Noetherian Ring|noetherian]], then only finitely many [[Prime Ideal|primes]] [[Contraction|contract]] to each $P \in \Spec(R)$[^1]. 

##### *Proof.*
If $Q' \in \Spec(S)$ contracts to $P$, then $Q' \supseteq P S$, so in particular $Q'$ contains some prime $Q$ minimal over $P S$. Then $$P S \subseteq Q \subseteq Q' \implies P \subseteq Q \cap R \subseteq Q' \cap R = P,$$so $Q' \cap R = Q \cap R$. By \hyperref[incomparability]{Incomparability}, $Q = Q'$. So all the primes contracting to $P$ are in $\Min(P S)$, which is a finite set since $R$ is noetherian, by \Cref{min primes finite}.

[^1]: Notation: [[Prime Spectrum]]