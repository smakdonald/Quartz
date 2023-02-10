### Problem 7 – Relatively Prime Extension (a)
Let $F \sse L$ be a [[Degree of Field Extension|finite]] [[Field Extension|extension]] of [[Field|fields]] and let $f(x) \in F[x]$ be an [[Irreducible|irreducible]] polynomial of [[Polynomial Degree|degree]] $d$. Prove that, if $\gcd(d,[L : F ]) = 1$, then $f (x)$ is also irreducible in $L[x]$.

##### *Proof*.
Let $F \sse L$ be a finite extension of fields and let $f(x) \in F[x]$ be an irreducible polynomial of degree $d$ such that $\gcd(d,[L : F ]) = 1$. Let $[L:F]=n$

First, note that if $d=1$ then $f$ is always irreducible, so we may reduce to the case where $d>1$. 

Let $K$ denote the algebraic closure of $F$, let $\a$ be a root of $f\in K$, and consider $F(\a)$ and $L(\a)$. Let $g(x)$ denote the minimal polynomial of $\a\in L(\a)$, and let $\deg(g)=q$. Thus $[L(\a):L]=q$. By the Degree Formula we have 
- $[L(\a):F]=[L(\a):L][L:F]=qn$
- $[L(\a):F]=[L(\a):F(a)][F(a):F]=md$ for some $m\in \N$.
Thus $qn=md$ and $md|qn$ As $n$ and $d$ are relatively prime we have $d|q$. However, $q$ is the minimal polynomial of $\a$, and thus $q\leq d$, yielding $q=d$. Thus $f=kg$ for some $k\in F$. As irreducible polynomials multiplied by a constant are still irreducible, we see that $f$ is indeed irreducible in $K[x]$.
***
#qual