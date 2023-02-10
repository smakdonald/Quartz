#### $\thm$ – Min Contained in Ass
Let $R$ be [[Noetherian Ring|noetherian]] and $M$ be an $R$-module. If $M$ is a finitely generated $R$-module, then $\Min(\ann_R(M))\subseteq \Ass_R(M)$[^1]. In particular, $\Min(I)\subseteq \Ass_R(R/I)$.

##### *Proof.*
By \Cref{supp v ass primes},$$V(\ann_R(M))=\Supp_R(M)=\bigcup_{P \in \Ass(M)} V(P),$$
so the minimal elements of both sets agree. In particular, the right hand side has the minimal primes of $\ann_R(M)$ as minimal elements, and they must be associated primes of $M$, or else this would contradict minimality.

[^1]: Notation: [[Minimal Prime]], [[Annihilator]], [[Associated Prime]]