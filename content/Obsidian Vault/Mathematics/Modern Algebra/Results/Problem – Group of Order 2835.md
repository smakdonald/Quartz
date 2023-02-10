### Problem 2 – Group of Order 2835
Let $G$ be a [[Group|group]] of [[Order|order]] $2835 = 3^4\cdot 5\cdot 7$.

(a) Show that there are at most two options for $n_3$, the number of [[Sylow p-Subgroup|Sylow]] $3$-subgroups of $G,$ and list them.
(b) Prove that $G$ is not [[Simple Group|simple]].

##### *Proof*.
Let $G$ be a group of order $2835$.

###### Part (a)
By [[Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]] we know that $n_3=1\mod{3}$ and $n_3|35$. The possible options are thus $1$ and $7$. 
***
###### Part (b)
Suppose by way of contradiction that $G$ is simple. Thus $n_3\neq 1$, so $n_3=7$. Let $G$ [[Group Action|act]] on the $\Syl_3(G)$ by conjugation, yielding the [[Homomorphism|homomorphism]] $$\rho: G\to S_7$$granted via the [[Proposition – Permutation Representation|permutation representation]]. By (2) in Sylow's Theorem we see that $\rho$ is not trivial. As $|S_7|=7!$ we see that $|G|\not\big||S_7|$, meaning that the $\ker(\rho)$ is non-trivial, yielding a non-trivial normal subgroup of $G$, a contradiction.
***
#qual