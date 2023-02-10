### Problem 1 – Group of Order 150
Prove that no [[Group|group]] of order 150 is [[Simple Group|simple]].

##### *Proof.*
Let $G$ be a group of order $150$ and suppose by way of contradiction that $G$ is simple. Notice that $150=2\cdot 3\cdot 5^2$. 
By [[Results#Theorem – Main Theorem of Sylow Theory|Sylow's Theorem]], we have the following:
- $|\Syl_5(G)|\equiv 1\mod{5}$ and divides $6$, the only options are thus $1$ and $6$. 
Since $G$ is simple, there must be exactly $n_5=6$, where $n_5=\Syl_5(G)$. Let $G$ [[Group Action|act]] on $\Syl_5(G)$ by conjugation. Thus $\rho: G\to S_6$ is a group homomorphism. Note that $|S_6|=720$, and that the order of $G$ does not divide $720$. By part (2) of Sylow's Theorem this action is [[Transitive Action|transitive]], meaning that the [[Kernel|kernel]] of $\rho$ cannot be trivial. $\ker(\rho)$  is a nontrivial normal subgroup of $G$, a contradiction. Thus no group of order $150$ is simple.
***
#qual