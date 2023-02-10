#### $\thm$ – Supp v Ass Primes
Let $R$ be [[Noetherian Ring|noetherian]] and $M$ be an $R$-module.[^1] 
$$\Supp(M) \,\, = \displaystyle\bigcup_{P \in \Ass(M)} V(P).$$
##### *Proof.*
Let $P \in \Ass_R(M)$, and fix $m \in M$ such that $P = \ann_R(m)$. Let $Q \in V(P)$. By \Cref{supp v ann}, $Q \in \Supp(R/P)$. Since $0 \to R/P \xrightarrow{m} M$ is exact and localization is exact, by \Cref{localization is exact}, $0 \to (R/P)_Q \to M_{Q}$ is also exact. Since $(R/P)_Q \neq 0$, we must also have $M_{Q} \neq 0$, and thus $Q \in \Supp(M)$. This shows $\Supp(M) \, \supseteq \displaystyle\bigcup_{P \in \Ass(M)} V(P)$.
Now let $Q$ be a prime ideal and suppose that $$Q \notin \bigcup_{P\in \Ass(M)} V(P).$$ In particular, $Q$ does not contain any associated prime of $M$. Then there is no associated prime of $M$ that does not intersect $R \setminus Q$, so by \Cref{associated primes localize}, $\Ass_{R_{Q}}(M_{Q})=\varnothing$. By \Cref{associated primes nonzero}, $M_{Q}=0$.

[^1]: Notation: [[Support]], [[Associated Prime]], [[V(I)]]