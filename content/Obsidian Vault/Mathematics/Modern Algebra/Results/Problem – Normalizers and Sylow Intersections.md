### Problem 3 – Normalizers and Sylow Intersections 
Let $G$ be a [[Group|group]] of [[Order|order]] $90 = 2 · 3^2 · 5$ and let $\Syl_3(G)$ denote the set of  
[[Sylow p-Subgroup|Sylow]] $3$-subgroups of $G$.

(a) Suppose for any $Q, Q' \in \Syl_3(G)$ either $Q = Q′$ or $Q \cap Q' = {1}.$ Prove that $G$ is not [[Simple Group|simple]].
(b) Suppose there exists $Q, Q' ∈ \Syl_3(G)$ such that $|Q \cap Q'| = 3$. Prove that $G$ is not simple. (Hint: Consider the [[Centralizer & Normalizer|normalizer]] of $Q \cap Q'$.)

##### *Proof.*
Let $G$ be a group of order $90 = 2 · 3^2 · 5$ and let $\Syl_3(G)$ denote the set of  
Sylow $3$-subgroups of $G$.
###### Part (a)
Suppose by way of contradiction that $G$ is simple. 
By Sylow's Theorem we know the following:
- $n_3|10$ and is congruent to $1\mod{3}$. As $G$ is simple there must be ten of the fuckers. 
- $n_5|18$ and is congruent to $1\mod 5$. As $G$ is simple there must be six of them. 
Since each Sylow $3$-subgroup will have $3^2-1=8$ non-identity elements and they are all distinct that accounts for $80$ elements of order $3$. However, there are also $24$ elements or order $5$ to account for, which is a problem. Thus $G$ cannot be simple. 
***
###### Part (b)
Suppose now that there exists $Q, Q' ∈ \Syl_3(G)$ such that $|Q \cap Q'| = 3$. . Given this intersection, we know that $|QQ'|=9\cdot 9/3=27$. Additionally, note that as $Q \cap Q'$ is a subgroup of both $Q$ and $Q'$ with index 3 in both, the smallest prime dividing the order or both, that $Q \cap Q'$ is normal in both.

We now consider the normalizer of $Q \cap Q'$, which we denote $N$ for simplicity. As $N$ is a subgroup of $G$ its order must divide $90$ by Lagrange's Theorem. However, $QQ'\leq N$, and so $N$ must have at least $27$ elements, leaving the options of $45$ and $90$. If $|N|=90$ then $N=G$, making $Q\cap Q'$ normal in $G$, a problem. 

If $|N|=45$ then $[G:N]=2$, the smallest prime dividing $G$. Thus $N$ is still normal, which is still a problem. Thus $G$ cannot be simple. 
***
#qual