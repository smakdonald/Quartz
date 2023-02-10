### Problem 2 – Unique Proper Normal Subgroup
Let $G$ be a [[Order|finite]] [[Group|group]].

(a) If $N$ is a [[Normal Subgroup|normal]] [[Subgroup|subgroup]] of $G$ and $|N | = 2$, prove that $N$ is contained in the [[Center|center]] $Z(G)$ of $G$.
(b) Suppose that $| Z(G)|$ is odd and that $G$ contains a non-trivial [[Simple Group|simple]] subgroup $H$ with $[G : H] = 2$[^1]. Prove that $H$ is the only non-trivial proper normal subgroup of $G$.

##### *Proof.*
##### Part (a)
Let $x\in N$ and let $g\in G$. As $N$ is normal, we see $gxg\inv\in N$, and thus one of the following must be true:
- $gxg\inv=e$, where $e$ is the identity element of $G$, or
- $gxg\inv=x$, the only other element of $N$.
However, in the first case we would have $x=e$ by multiplying $g$ and $g\inv$ over, and thus it must be the case that $gxg\inv=x$, or $gx=xg$. Thus $x\in Z(G)$. 
***
###### Part (b)
From [[Theorem – Lagrange's Theorem|Lagrange's Theorem]] we know that $|G|/|H|=2$, meaning that $G$ has an even number of elements. Thus $2$ is the smallest prime dividing the order of $G$, making $H$ normal in $G$ (See: ). 

Suppose by way of contradiction there exists some non-trivial proper normal subgroup $N$ of $G$ that is not $H$. As $H$ is normal, by the [[Theorem – Second Isomorphism Theorem|Second Isomorphism Theorem]] we have $H\cap N\nsg H$. However, as $H$ is simple, this means that $H\cap N=\{e\}$. SIT also tells us that $HN\leq G$. As $|H|=|G|/2$, this makes $|N|=2$ and $G=HN$. From part (a), $N\leq Z(G)$. However, this contradicts Lagrange's Theorem, as $2$ does not divide any odd numbers.
***
#qual

[^1]: Notation: [[Index]]