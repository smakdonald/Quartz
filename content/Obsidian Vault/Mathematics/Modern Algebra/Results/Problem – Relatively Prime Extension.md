### Problem 7 – Relatively Prime Extension
Assume that $F \sse K$ is a [[Degree of Field Extension|finite]] [[Field Extension|extension]] of [[Field|fields]] of [[Degree of Field Extension|degree]] $n = [K : F ]$.

(a) Prove that if $f \in F [x]$ is [[Irreducible|irreducible]] of [[Polynomial Degree|degree]] $d$ and $\gcd(d, n) = 1$ then $f$ remains  
irreducible when regarded as an element of the ring $K[x]$.
(b) Show, by means of an explicit example with justification, that the statement in  
part (a) would become false if the assumption that $\gcd(n, d) = 1$ were omitted.

##### *Proof.*
Let $F \subseteq K$ be a finite extension of fields of degree $n = [K : F ]$.

###### Part (a)
Suppose that $f \in F[x]$ is irreducible of degree $d$ and $\gcd(d, n) = 1$. 

First, note that if $d=1$ then $f(x)$ will remain irreducible in $K[x]$ (See: [[Theorem – Degree and Irreducibility|Theorem]]).
Suppose then that $d>1$. There exists an [[Algebraically Closed|algebraically closed]] extension $\widetilde F$ such that $f$ has a root $r$ (See: [[Theorem – Existence and Uniqueness of Algebraic Closures|Theorem]]). Consider $K(r)$. As $r$ is [[Algebraic Element|algebraic]] in $K(r)$ we know there exists some unique irreducible [[Minimum Polynomial|minimal polynomial]] $g$ of degree $q$, and thus that $[K(r):K]=q$ (See: [[Theorem – Properties of Algebraic Elements|Theorem]]). Using the [[Proposition – The Degree Formula|Degree Formula]] we see that $$[K(r):F]=[K(r):K][K:F]=qn.$$However, $[K(r):F]=[K(r):F(r)][F(r):F]$ and so $qn=md$ for some $m\in\Z$, so $d|qn$. As $\gcd(n,d)=1$ we must have $d|q$. But $q$ was defined to be the degree of $g$, which divides $f$. As $d|q$ and $q\leq d$, we see that $d=q$, so so $f=kg$ for some $k\in F$. As irreducible polynomials multiplied by a constant are still irreducible, we see that $f$ is indeed irreducible in $K[x]$.
***
###### Part (b)
Let $p(x)$ be a non-constant irreducible polynomial of degree $d$ in $F[x]$. Let $K=F[x]/p(x)$. Because $p(x)$ is irreducible and $F[x]$ is a PID, $(p(x))$ is a maximal ideal. Thus $K = F[x]/(p(x))$ is a field (See: [[Theorem – Prime, Maximal, Domain, Field|Theorem]]), $[K:F]=d$, and $x+p(x)$ is a root of $p(x)$ in $K$ (See: [[Proposition – Properties of Extension Degrees|Proposition]]). Hence $p(x)$ is no longer irreducible by Theorem 2.2.
***
#qual