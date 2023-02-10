### Problem 3 – Group of Order 1683 Abelian
Prove that any group of order $3^2\cdot 11\cdot 17$ is abelian.

##### *Proof.*
Let $G$ be a group of order $3^2\cdot 11\cdot 17$. By Sylow's Theorem we see the following:
- $n_{11}|153$ and $n_{11}\equiv 1\mod{11}$, and so $n_{11}=1$.
- $n_{17}|99$ and $n_{17}\equiv 1\mod{17}$, and so $n_{17}=1$ as well.
- $n_3|187$ and $n_3\cong 1\mod{3}$, so actually $n_3=1$ too. 
Thus the unique Sylow $11$-subgroup and Sylow $17$-subgroup, denoted $P$ and $Q$, respectively, are normal in $G$. 

As $P$ and $Q$ are normal in $G$ and intersect trivially, we see that $PQ\leq G$. Let $g\in G$ and consider $gPQg\inv$. Let $pq\in PQ$ and notice $g(pq)g\inv=gpg\inv gqg\inv$. As $p\in P\nsg G$ and $q\in Q\nsg G$ we see $gpg\inv\in P$ and $gqg\inv\in Q$, thus $gpqg\inv\in PQ$, making $PQ\nsg G$. 

Let $R$ be the unique Sylow $3$-subgroup, which has order $9$. As $R\nsg G$ and intersects with $PQ$ trivially, we see $G=PQ\times R$, a direct product of cyclic groups of relatively prime order, making $G$ abelian.
***
#qual