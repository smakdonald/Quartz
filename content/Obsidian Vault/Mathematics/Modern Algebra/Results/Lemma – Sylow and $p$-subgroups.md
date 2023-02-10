#### $\lem$ – Sylow and $p$-subgroups
Let $G$ be a [[Order|finite]] [[Group|group]], $p$ a prime, $P$ a [[Sylow p-Subgroup|Sylow]] $p$-[[Subgroup|subgroup]] of $G$, and $Q$ any $p$-subgroup of $G$. Then $Q \cap N_G(P) = Q \cap P$.[^1]

###### *Proof.* 
Since $P \leq N_G(P)$, we have $$Q \cap P \leq Q \cap N_G(P).$$For the reverse containment, let $H =  Q \cap N_G(P).$ Since $H \subseteq N_G(P)$, we have that $PH=HP$ so $PH$ is a subgroup of $G$ by Exercise \ref{ex:HK=KH}. Also by Corollary \ref{cor:|HN|} we have $$|PH| = \frac{|P| |H|}{|P \cap H|} $$and since each of $|P|$, $|H|$, and $|P \cap H|$ is a power of $p$, $PH$ is a $p$-subgroup of $G$. But $P \leq PH$ and $P$ is a $p$-subgroup of largest possible order. So $P = PH$. This proves $H \leq P$ and thus $H \leq Q\cap P$.
***

[^1]: For $N_G(P)$, See: [[Centralizer & Normalizer|Normalizer]]