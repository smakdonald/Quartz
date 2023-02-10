### Problem 4 – Prime Ideals Maximal in Finite Rings
Let $R$ be a [[Commutative Ring|commutative]] [[Ring|ring]] with [[Unital Ring|identity]], and assume $1\neq0$.

(a) Prove that every [[Mathematics/Modern Algebra/Definitions/Maximal Ideal|maximal]] ideal of $R$ is a [[Mathematics/Modern Algebra/Definitions/Prime Ideal|prime ideal]].
(b) Assume $R$ is a finite ring. Prove that every prime ideal is a maximal ideal.

##### *Proof.*
###### Part (a)
Let $M$ be a maximal ideal of $R$. We show that $R/M$ is a field (See: [[Theorem – Prime, Maximal, Domain, Field|Theorem]]). By the [[Theorem – The Lattice Isomorphism Theorem|Lattice Isomorphism Theorem]] we know there is a one-to-one correspondence between the ideals of $R/M$ and the ideals of $R$ containing $M$. However, as $M$ is maximal, the only ideals of $R$ containing $M$ are $R$ and $M$ itself, meaning that $R/M$ has exactly two ideals, making $R/M$ a field. 

We show that since $R/M$ is a domain, $M$ must be prime. (See: [[Theorem – Prime, Maximal, Domain, Field|Theorem]]). Suppose by way of contradiction that $M$ is not prime, so exist elements $x,y\in R$ such that $xy\in M$ but neither $x$ nor $y$ are in $M$. Thus $xM\cdot yM=xyM=M$, making $x$ and $y$ zero-divisors in $R/M$, contradicting the fact that $R/M$ is a field. Thus $M$ is prime.
***
###### Part (b)

Let $R$ be a finite ring, and let $P$ be a prime ideal in $R$. We show $R/P$, a finite integral domain, is a field (See: ) Let $a\not\in P$, and consider $a^n$ for all $n\in\N$. As $R/P$ is finite, there exists some $k<m\in N$ such that $a^k=a^m$. Then $a^{m-k}\cdot a^k=a^m=a^k$, meaning that $a^{m-k}=e$. Thus $a$ has inverse $a^{m-k-1}$, making $a$ a unit. Thus $R/P$ is a field, making $P$ a maximal ideal (See: [[Theorem – Prime, Maximal, Domain, Field|Theorem]])
***
#qual