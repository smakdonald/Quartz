#### $\lem$ – Min Primes Intersection All Important
If $\Min(I) = \{ P_1, \ldots, P_n \}$[^1], no $P_i$ can be deleted in the intersection $P_1 \cap \cdots \cap P_n$. 

##### *Proof.*
Suppose that we can delete $P_i$, meaning that $$\bigcap_{j=1}^n P_j = \bigcap_{j \neq i} P_j.$$Then $$P_i \supseteq \bigcap_{j=1}^n P_j = \bigcap_{j \neq i} P_j \supseteq \prod_{j \neq i} P_j.$$Since $P_i$ is prime, this implies that $P_i \supseteq P_j$ for some $j \neq i$, but this contradicts the assumption that the primes are incomparable.

[^1]: Notation: [[Minimal Prime]]