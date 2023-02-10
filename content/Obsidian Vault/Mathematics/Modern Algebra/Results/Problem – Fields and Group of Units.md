### Problem 6 – Fields and Group of Units 
Let $F$ be a [[Field|field]] and $G$ a [[Order|finite]] [[Subgroup|subgroup]] of the multiplicative group $F^∗$.  
Prove that $G$ is [[Cyclic|cyclic]].

##### *Proof*.
Let $F$ be a field and $G$ a finite subgroup of order $n$ the multiplicative group $F^∗$. Let $k$ denote the LCM of all orders of elements in $G$. Notice that as $g^n=1$ for all $g\in G$ we have $k\leq n$. 

However, as $g^k=1$ for all $g\in G$ we know that $g$ is the root of the polynomial $f(x)=x^k-1$ in $F[x]$. By the Factor Theorem there are thus at most $k$ roots of $f$, but there are $n$ distinct roots. Thus $k=n$. 

Thus the LCM of all orders of elements in $G$ is $n$. Notice that as $G$ is abelian every Sylow $p$-subgroup of $G$ is normal, and thus there is only one of each. This means that e$G$ can be written as a direct product of cyclic groups of relatively prime order, Thus $G$ is itself cyclic. 
***
#qual