### Problem 3 – Normalizer of Normalizer of Sylow Group
Let $G$ be a [[Order|finite]] [[Group|group]] and $p$ a prime dividing the order of $G$. Let P be a [[Sylow p-Subgroup|Sylow]] $p$-subgroup.
(a) Suppose $Q$ is a Sylow $p$-subgroup distinct from $P$. Prove that $PQ$[^1] is not a subgroup of $G$. (Recall that $PQ = {pq | p ∈ P, q ∈ Q}$.)
(b) Prove that $N_G(P ) = N_G(N_G(P ))$ where $N_G(H)$ denotes the [[Centralizer & Normalizer|normalizer]] in $G$ of a subgroup $H$.

##### *Proof.*
Let $G$ be a finite group and $p$ a prime dividing the order of $G$. Let P be a Sylow $p$-subgroup.

###### Part (a)
We proceed via the contrapositive.
Let $Q$ be a Sylow $p$-subgroup, and suppose $PQ\leq G$. Thus $|PG|\big||G|$

Note that $P$ and $Q$ both have $p^k$ elements, where $p^k$ is the largest power of $p$ that divides the order of $G$. Recall $|PQ|=\frac{|P||Q|}{|P\cap Q|}=\frac{p^{2k}}{|P\cap Q|}$. As $p^k$ is the largest power of $p$ that divides the order of $G$, we see that $|P\cap Q|$ must be at least $p^k$. Thus $P=Q$. 
***
###### Part (b)
First, note that $P\leq N_{G}(P)\leq N_G(N_G(P))$. Note that $N_G(P)$ is the largest subgroup of $G$ such that $P$ is normal in $G$, making $P$ the only Sylow $p$-subgroup of $N_G(P)$. Let $x\in N_G(N_G(P))$. Notice that $xPx\inv\leq xN_G(P)x\inv$, but as $x\in N_G(N_G(P))$ we have $xN_G(P)x\inv=N_G(P)$. As $xPx\inv$ is a Sylow $p$-subgroup that is contained in $N_G(P)$, we see that $xPx\inv=P$, placing $x\in N_G(P)$. Thus $N_G(P)=N_G(N_G(P))$.
***
#qual

[^1]: Notation: [[HK]]