### Problem 2 – Sylow Group Contained in Center
Let $G$ be a [[Group|group]] of [[Order|order]] $385 = 5 · 7 · 11$. Prove that $G$ has a [[Normal Subgroup|normal]] [[Subgroup|subgroup]] of order $11$ and that the [[Center|center]] of $G$ contains a subgroup of order $7.$

##### *Proof*
Let $G$ be a group of order $385 = 5 · 7 · 11$. By Sylow's Theorem we know the $n_{11}|35$ and $n_11\equiv 1\mod{11}$, and so $n_{11}=1$, making $P$, the unique Sylow $11$-subgroup of $G$, normal in $G$. Things are looking good thus far.
We also know the following:
- $n_7|55$ and $n_7\equiv 1\mod{7}$, so $n_7=1$ as well. Yeehaw.

Let $P$ denote the unique Sylow $7$-subgroup, and let $G$ act on $P$ by conjugation. Thus $\rho:G\to S_7$. The First Isomorphism Theorem tells us that $G/K\cong\im(\rho)\leq\Aut(P)$, where $K$ is the kernel of $\rho$. However, $\Aut(P)=\Z_{7}^\times=\Z_6$, meaning that the order of $K$ must divide both $385$ and $6$, which cannot happen. Thus $K$ must be trivial, meaning that $gxg\inv=x$ for every $g\in G$ and $x\in P$, making $P$ a subgroup of $Z(G)$ of order $7$.
***
#qual