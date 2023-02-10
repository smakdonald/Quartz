### Problem 3 – Classify Groups of Order $3p$
Let $p$ be any positive prime integer. Prove that the number of [[Group|groups]] of order $3\cdot p$, up to [[Isomorphism|isomorphism]], is exactly
$$\begin{cases} 2, \text{ when }p = 2, p = 3, \text{ or }p\equiv 1 \mod 3, \text{ and }\\ 1, \text{ otherwise }\end{cases}$$
##### *Proof.*
Let $p$ be any positive prime integer.

First, suppose $p=2$. Thus $G$ is a group of order $pq$, making it abelian. So the only groups of order $6$ are $\Z_2\times\Z_3$ and $\Z_6$. The same applies when $p=2$, where the groups are $\Z_3\times\Z_3$ and $\Z_9$. 

Let $P$ be a Sylow $p$-subgroup of $G$, and note that $[G:P]=3$, the smallest prime dividing the order of $G$, making $P\nsg G$. Let $Q$ denote a Sylow $3$-subgroup of $G$. 
As $P$ and $Q$ are groups of relatively prime order we have $PQ=G$ and thus $G\cong P\sdp_\rho Q$, where $\rho:Q\to\Aut(P)$. Notice that since $|P|=p$, we have $\Aut(P)\cong\Z^{\times}_p\cong\Z_{p-1}$. Thus, by the First Isomorphism Theorem $Q/\ker(\rho)\cong\im(\rho)\leq\Z_{p-1}.$ As $Q$ has three elements, the kernel of $\rho$ must be either all of $Q$ or trivial. However, the order of the image must divide $\Z_{p-1}$, which is only possible when $p\equiv 1 \mod 3$. Thus when this is the case there are two groups of order $3p$, otherwise the kernel is always trivial and we have $G=P\times Q$ as the only group.
***
#qual