### Problem 5 – Irreducible Quartic and $p=k^2+1$
Let $p$ be any positive prime integer.

(a) Prove that if $p = k^2 + 1$ for some integer k, then p is not an [[Irreducible|irreducible]] element of $\Z[i]$.
(b) Prove $x^4-p$ is [[Irreducible|irreducible]] in $\Q(i)[x]$.

##### *Proof*.
Let $p$ be any positive prime integer.

###### Part (a)
Suppose $p = k^2 + 1$ for some integer $k$.  As $(k-i)(k+i)=p$, $p$ is not an irreducible element of $\Z[i]$.
***
###### Part (b) 
As $x^4-p$ is irreducible in $Q$ (Eisenstein, $p=p$) and $x^4-p$ is monic, we see that $[\Q(\sqrt[4]{p}):\Q]=4$. As $x^2+1$ is irreducible and monic, we see that $[\Q(\sqrt[4]{p},i):\Q(\sqrt[4]{p})]=2$. By the Degree Formula we have $[\Q(\sqrt[4]{p},i):\Q]=8$. Note that the four roots of $(x^4 - p)$ are the following:
- $\sqrt[4]{p}$, 
- $-\sqrt[4]{p}$,
- $\sqrt[4]{p}i,$ and 
- $-\sqrt[4]{p}i$.
As $\frac{\sqrt[4]{p}i}{\sqrt[4]{p}}=i$, we see that $\Q(\sqrt[4]{p})$ is the splitting field of $F$. Note then that as $[\Q(i):\Q]=2$ and the degree of the splitting field is 8, by the Degree Formula we see that the degree of the splitting field of $x^4-p$ over $\Q(i)=4$. As $x^4-p$ is monic and degree $4$, it must be the minimal polynomial of the second extension and thus irreducible in $\Q(i)[x]$.
***
#qual