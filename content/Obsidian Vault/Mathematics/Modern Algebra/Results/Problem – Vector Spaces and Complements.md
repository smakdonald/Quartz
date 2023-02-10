### Problem 9 – Vector Spaces and Complements
Let $F$ be a [[Field|field]], $V$ an $F$-[[Vector Space|vector space]], and $W$ a subspace of $V$. A subspace $U$ of $V$ is called  a *complement* of $W$ in $V$ if $V$ is the internal [[Direct Product, Sum|direct sum]] of $W$ and $U$ ; that is, $V=W\oplus U$.

(a) Prove that for every $V$ and $W$ as above, $W$ has at least one complement in $V$.
(b) Prove that if $U$ is a complement of $W$ in $V$ and $V$ is [[Dim (Vector Space)|finite dimensional]], then  $\dim_F (V ) = \dim_F (W ) + \dim_F (U )$ (where $\dim_F$ denotes the dimension of an $F$-vector space).

##### *Proof*.
Let $F$ be a field, $V$ an $F$-vector space, and $W$ a subspace of $V$.

###### Part (a)
Let $A$ denote the set of all subspaces of $V$ such that $A\cap W=\{0\}$. We can order $A$ with respect to inclusion. Let $X$ be a totally ordered subset of $A$, and let $B$ be the union of all the elements in $X$. Unions of subspaces are subspaces, and by DeMorgan's Laws we see that $B\cap W=\{0\}$. Thus by Zorn's Lemma there exists a maximal element of $A,$ which we denote $U$. So $U\cap W=\{0\}$ by definition. 

Suppose by way of contradiction there exists some $x\in V$ such that $x\not\in U+W$.

Consider $U+Vx$. As $x\not\in W$, $vx\not\in W$ for all $v\in V$, as we could just multiply by $v\inv$. Thus $W\cap U+Vx=\{0\}$ and $U\subsetneq U+Vx$, a contradiction, as $U$ was maximal. Thus $U$ is a complement of $W$.
***
###### Part (b) 
The Second Isomorphism Theorem tells us that $U+W/W\cong U/(U\cap W)$. We also know that $$\dim(U)-\dim(U\cap W)=\dim(U/U\cap W)=\dim(U+W/W)=\dim(U+W)-\dim(W).$$
Put succinctly, $$\dim(U)-\dim(U\cap W)=\dim(U+W)-\dim(W),$$ and thus $$\dim(U)+\dim(W)=\dim(U+W)+\dim(U\cap W).$$ As $U\cap W=\{0\}$, we see that $\dim_F(V)=\dim_F(W)+\dim_F(U)$.
***
#qual