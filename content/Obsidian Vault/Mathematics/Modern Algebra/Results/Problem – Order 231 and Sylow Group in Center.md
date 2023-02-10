### Problem 1 – Order 231 and Sylow Group in Center
Let $G$ be a [[Group|group]] of [[Order|order]] $231(= 3 · 7 · 11)$

(a) Prove that $G$ has a unique $11$-[[Sylow p-Subgroup|Sylow]] subgroup
(b) Prove that the $11$-Sylow subgroup is contained in the [[Center|center]] of $G$.

##### *Proof.*
Let $G$ be a group of order $231(= 3^2 · 7 · 11)$

###### Part (a)
By [[Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]] we know $n_{11}|21$ and is congruent to $1\mod{11}$. The only possibility for such is $1$, meaning that $G$ has exactly $1$ Sylow $11$-subgroup.
***
###### Part (b)
Let $G$ [[Group Action|act]] on $P$ by conjugation. This gives rise to the [[Proposition – Permutation Representation|permutation representation]] [[Homomorphism|homomorphism]] $\rho: G\to S_{11}$. However, $P$ has prime order, making it a [[Cyclic|cyclic]] group [[Isomorphism|isomorphic]] to $\Z_{11}$. 

By the [[Theorem – First Isomorphism Theorem|First Isomorphism Theorem]] we know that $G/\Ker(\rho)\cong\im(\rho)=\Aut(P)$. However, $\Aut(P)\cong\Aut(\Z_{11})\cong \Z^x$, which has order $10$.  As this is a homomorphism, we see the order of $G/\ker(\rho)$ must divide both $10$ and $231$, two numbers that are relatively prime. Thus $\ker(\rho)=1$, meaning that conjugation is equivalent to the identity map, or that $gxg\inv=x$ for all $g\in G$. Thus $P\in Z(G)$.
***
#qual