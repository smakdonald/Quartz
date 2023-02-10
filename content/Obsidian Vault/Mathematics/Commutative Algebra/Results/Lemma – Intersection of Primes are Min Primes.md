#### $\lem$ – Intersection of Primes are Min Primes
Let $I$ be an ideal in $R$. If $I = P_1 \cap \cdots \cap P_n$ where each $P_i$ is [[Prime Ideal|prime]] and $P_i \not\subseteq P_j$ for each $i \neq j$, then $\Min(I)=\{ P_1, \ldots, P_n\}$[^1]. Moreover, $I$ must be [[Radical Ideal|radical]].

##### *Proof.*
If $Q$ is a prime containing $I$, then $Q \supseteq (P_1 \cap \cdots \cap P_n)$. We claim that $Q$ must contain one of the $P_i$. Indeed, if $Q \not\supseteq P_i$ for all $i$, then there are elements $f_i \in P_i$ such that $f_i \notin Q$, so their product satisfies $f_1 \cdots f_n \in (P_1 \cap \cdots \cap P_n)$ but $f_1 \cdots f_n \notin Q$. This is a contradiction, so indeed any prime containing $I$ must contain some $P_i$. Therefore, any minimal prime of $I$ must be one of the $P_i$. Since we assumed that the $P_i$ are incomparable, these are exactly all the minimal primes of $I$.
By assumption, $I$ coincides with the intersection of its minimal primes, which is $\sqrt{I}$ by \Cref{spectrum analogue nullstellensatz}. Therefore, $I = \sqrt{I}$.

[^1]: Notation: [[Minimal Prime]]