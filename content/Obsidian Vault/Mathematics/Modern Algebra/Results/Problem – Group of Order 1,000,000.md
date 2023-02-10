### Problem 3 – Group of Order 1,000,000
Let $G$ be a [[Group|group]] and let $n_p$ be the number of [[Sylow p-Subgroup|Sylow]] $p$-subgroups of $G$, where $p$ is a  
prime dividing the [[Order|order]] of $G$.
(a) Prove that if $G$ is [[Simple Group|simple]] then $|G|\big|n_p!$
(b) Deduce that there is no [[Simple Group|simple]] group of [[Order|order]] $1,000,000$.

##### *Proof.*
Let $G$ be a group, $p$ a prime dividing the order of $G$, and $n_p$ the number of Sylow $p$-subgroups of $G$.

###### Part (a) 
Let $G$ [[Group Action|act]] on $\Syl_p(G)$ by conjugation, inducing the [[Homomorphism|homomorphism]] $\rho: G\to S_{n_p}$ via the [[Proposition – Permutation Representation|permutation representation]]. Notice that the order of $S_{n_p}$ is conspicuously $n_p!$. The [[Kernel|kernel]] of this map is a [[Normal Subgroup|normal]] subgroup of $G$ (See: [[Corollary – Normal iff Kernel of Homomorphism|Corollary]]). However, since $G$ is simple, the only normal subgroups of $G$ are the trivial subgroup and $G$ itself. However, the kernel cannot be all of $G$ as this would make $\rho$ trivial, which cannot be the case given that our action is [[Transitive Action|transitive]] by part (2) of [[Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]]. Thus $\ker(\rho)=\{e\}$, making $\rho$ injective. Thus $|\im(\rho)|=|G|$. As the image is a subgroup of $S_{n_p}$, the result follows from [[Theorem – Lagrange's Theorem|Lagrange's Theorem]].
***
###### Part (b)
Let $G$ be a group of order $1,000,000$. Suppose by way of contradiction that $G$ is simple. $1,000,000=10^6=2^6\cdot 5^6$. Thus the number of [[Sylow p-Subgroup|Sylow]]-$5$ subgroups is congruent to $1\mod 5$ and divides $2^6=64$, the options of which are 1 and 16 (See: [[Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]]). As $|G|$ does not divide $16!$, this contradicts part (a). Thus there are no simple groups of order $1,000,000$.

#qual