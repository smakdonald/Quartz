### Problem 4 – Prime Ideal with Finite Index

(a) Prove that a finite [[Integral Domain|integral domain]] $D$ must be a [[Field|field]].
(b) Prove that if $R$ is a [[Commutative Ring|commutative]] [[Ring|ring]] and $P\subseteq R$ is a [[Prime Ideal|prime]] [[Ideal|ideal]] such that $P$ has finite [[Index|index]] as an additive [[Subgroup|subgroup]] of $R$, then $P$ is a [[Mathematics/Modern Algebra/Definitions/Maximal Ideal|maximal]] ideal. Give an example to show that this implication may fail if the finite index assumption is dropped.

##### *Proof.*
###### Part (a) 
Let $D$ be a finite integral domain. 

Let $x\in D$, and consider the set $\{x^n|n\in\N\}$. As $D$ is finite there must exist $n<m\in\N$ such that $x^n=x^m$. In integral domains cancellation is allowed, and thus we can cancel an $x^n$ from both sides, yielding $e=x^{m-n}$, and thus $x\cdot x^{m-n-1}=e$, making $x$ a [[Unit|unit]] of $D$. Thus $D$ is a field.
***
###### Part (b)
Let $R$ be a commutative ring and $P\subseteq R$ a prime ideal such that $P$ has finite index as an additive subgroup of $R$. 

Consider $R/P$, which is a domain since $P$ is a prime ideal (See: [[Theorem – Prime, Maximal, Domain, Field|Theorem]]). As $[R:P]=n$ for some $n\in\N$, we know that $|R/P|=n$, making it a finite domain. Thus $R/P$ is a field by Part (a), making $P$ maximal by the same theorem as above.

Let $R=\Z$ and consider $R[x]$, in which $(x)$ is a prime ideal. However, $R[x]/(x)=\Z$, which does not have finite order, nor is it a field.
***
#qual