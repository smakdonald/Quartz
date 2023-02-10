#### $\thm$ – Dimension Theorem
Any two [[Basis and Free Module|bases]] of the same [[Vector Space|vector space]] have the same [[Dim (Vector Space)|dimension]].

###### *Proof.* 
We will only prove this in the case of finite dimensional vector spaces, but it is indeed true in general. 

Suppose $F$ is a field and $V$ is a finite dimensional $F$-vector space.  Then it has a finite basis $B$. Let $B'$ be any other basis. (Note that we cannot assume $B'$ is necessarily finite.) For any non-negative integer $m$, suppose $C$ is any $m$-element subset of $B'$.
Then $C$ is linearly independent and so, by the Exchange Lemma \ref{lem:replacement}, there is an $m$-element subset $D$ of $B$ such that $(B \setminus D) \cup C$ is also a basis of $V$. In particular, $m \leq \# B$.  Since this holds for all $m$, we conclude $|B|' \leq  |B|$. By symmetry, $|B| \leq |B|'$ and hence $\# B= \# B'$.
***