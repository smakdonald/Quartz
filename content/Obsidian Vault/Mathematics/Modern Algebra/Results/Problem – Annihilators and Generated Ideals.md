### Problem 5 – Annihilators and Generated Ideals
Let $R$ be a (not-necessarily commutative) [[Ring|ring]] let $M$ be a left $R$-[[Module|module]]. The [[Annihilator|annihilator]] of $M$ in $R$ is defined to be $$\ann_R(M) = \{ r \in R \mid rm = 0 \text{ for all $m \in M$}\}.$$(a) Prove that $\ann_R(M)$ is a $2$-sided [[Ideal|ideal]] of $R$.
(b) Suppose $M$ is an [[Abelian Group|abelian]] [[Group|group]] (i.e., a $\Z$-[[Module|module]]) such that $|M| = 400$ and $\ann_\Z(M)$ is the ideal [[Generator|generated]] by $20$. How many possibilities, up to [[Isomorphism|isomorphism]], are there for $M$?

##### *Proof*.
###### Part (a)
Let $a,b\in \ann_R(M)$. Consider $(a+b)m=am+bm=0$. Thus $a+b\in \ann_R(M)$. Let $r\in\ann_R(M)$ and consider $-r$. Let $m\in M$ and suppose $-rm=n$ for some $n\in R$. Add $rm$ to both sides to see that $0=n+rm=n$. Thus $n=0$ and $-rm=0$ for all $m\in M$. So $-r\in\ann_R(M)$.

Note that as $0m=0=m0$ for all $m\in M$, we know that $0\in\ann_R(M)$. As $rm=0$ for all $m\in M$, we see that $\ann_R(M)$ is a left sided ideal.

Suppose $mr=n$ for some $m\in R$. This time we add $-rm$ to both sides, but as $-r\in\ann_R(M)$, we once again find that $mr=0$. Notice that this means $rm=mr$ for all $r\in \ann_R(M)$ and $m\in M$, and thus that elements of $\ann_R(M)$ commute with elements of $M$. 

Let $a,b\in \ann_R(M)$. Consider $m(a+b)=ma+mb$.  Luckily, we know $ma=am=0=bm=mb$, and thus that $ma+mb=0+0=0$. Hence $a+b\in \ann_R(M)$, making $\ann_R(M)$ is a two sided ideal. 
***
###### Part (b)
By the Fundamental Theorem of Finitely Generated Abelian Groups (Elementary Divisor Form) and Sun Tzu's Theorem, there are only so many options we have for $M$:
- $\Z_{16}\times \Z_{25}$, 
- $\Z_{8}\times \Z_{2}\times \Z_{25}$, 
- $\Z_{4}\times \Z_{4}\times \Z_{25}$, 
- $\Z_{4}\times \Z_{2}\times \Z_{2}\times \Z_{25}$, 
- $\Z_{2}\times\Z_{2}\times \Z_{2}\times \Z_{2}\times \Z_{25}$, 
- $\Z_{16}\times \Z_{5}\times \Z_{5}$, 
- $\Z_{8}\times \Z_{2}\times \Z_{5}\times \Z_{5}$,
- $\Z_{4}\times \Z_{5}\times \Z_{20}$
- $\Z_{4}\times \Z_{2}\times \Z_{2}\times \Z_{5}\times \Z_{5}$, and 
- $\Z_{2}\times\Z_{2}\times \Z_{5}\times \Z_{20}$.
However, as ideals are additive subgroups, we know that $M$ needs to contain a cyclic subgroup of order $20$. Thus we need only consider decompositions with a $\Z_{20}$ in them, of which there are exactly two:
1. $\Z_{4}\times \Z_{5}\times \Z_{20}$
2. $\Z_{2}\times\Z_{2}\times \Z_{5}\times \Z_{20}$
***
#qual