### Problem 7 – Splitting Field and Fifth Root of Unity
Let $L$ be the [[Splitting Field|splitting]] [[Field|field]] of $x^5 - 11$ over $\Q$

(a) Find, with justification, the [[Degree of Field Extension|degree]] of $L$ over $\Q$.
(b) Let $F = \Q(\zeta)$ where $\zeta = e^{2\pi i/5}$, a primitive $5\th$ root of unity. Prove $x^5 - 11$ is [[Irreducible|irreducible]] in $F[x]$.

##### *Proof*.
Let $L$ be the splitting field of $f(x)=x^5 - 11$ over $\Q$

###### Part (a)
First, notice that by [[Theorem – Eisenstein's Criterion|Eisenstein's Criterion]] ($p=11$) we have $f$ irreducible in $\Q$. 

The roots of $f$ are the following:
1. $\a_1=\sqrt[5]{11}\z$
2. $\a_2=\sqrt[5]{11}\z^2$
3. $\a_3=\sqrt[5]{11}\z^3$
4. $\a_4=\sqrt[5]{11}\z^4$
5. $\a_5=\sqrt[5]{11}\z^5=\sqrt[5]{11}$

As $f$ is monic and irreducible, it is the [[Minimum Polynomial|minimum polynomial]] of $\a_5$. Let $E=\Q(\a_5)$ and notice $[E:\Q]=5$. 

Notice that $\z$, a primitive $5$-th root of unity, is the root of $g(x)=x^4+x^3+x^2+x+1$, the fourth cyclotomic polynomial, which is monic and irreducible in $\Q[x]$ (See: [[Proposition – Cyclotomic Polynomial Irreducible|Result]]). Thus $g$ is the minimum polynomial of $\z$ and $[F:\Q]=4$. 

We know that $L=\Q(\sqrt[5]{11},\z)$, as every generator of $L$ can be written using $\z$ and $\sqrt[5]{11}.$ Let $[L:\Q]=n$, $[L:F]=p$, and $[L:E]=q$. By the [[Proposition – The Degree Formula|Degree Formula]], we have 
- $[L:\Q]=[L:F][F:\Q]$, and thus $n=4p$
- $[L:\Q]=[L:E][E:\Q]$, and thus $n=5q$
As $E\neq L$ and $F\neq L$ we know that $p,q>1$. 

Thus we have $n=20$. 
***
###### Part (b) 
Let $F = \Q(\zeta)$ where $\zeta = e^{2\pi i/5}$. From Part (a) we know $[L:F]=5$. As $L=F(\a)$, we know that $\mp_\a(x)$ has degree $5$. As $f$ is a monic polynomial of degree $5$, we see that it is the minimum polynomial and thus irreducible.

#qual