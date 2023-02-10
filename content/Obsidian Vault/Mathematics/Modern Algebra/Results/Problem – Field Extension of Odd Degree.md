### Problem 7 – Field Extension of Odd Degree
Suppose that $K/F$ is a [[Degree of Field Extension|finite]] [[Field Extension|extension]] of [[Field|fields]] such that the [[Degree of Field Extension|degree]] $[K : F ]$ is odd. Show  
that if $b \in K$, then $F (b) = F (b^2)$.

##### *Proof*.
Let $K/F$ be a finite extension of fields such that the degree $[K : F ]$ is odd. 

Notice that $F(b^2)\subseteq F(b)$ as everything in $b^2$ can be written in terms of $b$. 
Suppose by way of contradiction that there exists some $\a\in F(b)$ such that $\a\not\in F(b^2)$. Then $b\not\in F(b^2)$. Notice that $b$ is a root of the polynomial $f(x)=x^2-b^2\in F(b^2)$, which is irreducible in $F(b^2)$ as it is a degree $2$ polynomial that has no roots in $F(b^2)$. Thus $f$ is the minimum polynomial of $b$ and $[F(b):F(b^2)]=2$. 

However, by the Degree Formula $[K:F]=[K:F(b)][F(b):F(b^2)][F(b^2):F]$, which is a problem, given $2$ now divides $[K:F]$, an odd number. Thus $F (b) = F (b^2)$.
***
#qual