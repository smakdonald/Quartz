#### $\lem$ – Associated Prime and Localization
Let $R$ be a [[Noetherian Ring|noetherian ring]] and $M$ be an $R$-module. A [[Prime Ideal|prime]] $P$ is [[Associated Prime|associated]] to $M$ if and if and only if $P_P \in \Ass(M_P)$[^1].

##### *Proof.*
Localization is exact, by \Cref{localization is exact}, so any inclusion $R/P \subseteq M$ localizes to an inclusion $R_P/P_P \subseteq M_P$. Conversely, suppose that $P_P = \ann(\frac{m}{w})$ for some $\frac{m}{w} \in M_P$. Let $P = (f_1, \ldots, f_n)$. For each $i$, since $\frac{f_i}{1} \frac{m}{w} = \frac{0}{1}$, there exists $u_i \notin P$ such that $u_i f_i m = 0$. Then $u = u_1 \cdots u_n$ is not in $P$, since $P$ is prime, and $u f_i m = 0$ for all $i$. Since the $f_i$ generate $P$, we have $P (um) = 0$. On the other hand, if $r \in \ann(um)$, then $\frac{ru}{1} \in \ann(\frac{m}{w}) = P_P$. We conclude that $ru \in P_P \cap R = P$. Since $u \notin P$ and $P$ is prime, we conclude that $r \in P$.

[^1]: See: [[Localization]]