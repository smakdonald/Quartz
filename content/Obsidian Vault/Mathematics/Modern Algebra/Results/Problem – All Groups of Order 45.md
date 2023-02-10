### Problem 3 – All Groups of Order 45
Determine all of the [[Group|groups]] of [[Order|order]] $45$, up to [[Isomorphism|isomorphism]]

##### *Proof.*
By Sylow's Theorem we know the following:
- $n_3|5$ and $n_3\equiv 1\mod{3}$, so $n_3=1$. 
- $n_5|$ and $n_5\equiv1\mod{5}$, so $n_5=1$ as well. 
Thus there is exactly one Sylow $5$-subgroup, $P$, and exactly one Sylow $3$-subgroup, $Q$. Both are normal in $G$. Notice that $Q$ has order $9$, a prime squared. Thus $Q$ is abelian. By the Fundamental Theorem of Finitely Generated Abelian Groups, $Q$ is either isomorphic to $\Z_3\times\Z_3$ or $\Z_9$. Thus $G\cong\Z_5\times\Z_9$ or $G\cong\Z_5\times\Z_3\times\Z_3$.
***
#qual