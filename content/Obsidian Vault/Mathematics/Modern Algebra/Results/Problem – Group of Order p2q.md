### Problem 2 – Group of Order $p^2q$
Let $G$ be a [[Group|group]] of [[Order|order]] $p^2q$ where $p$ and $q$ are distinct primes.
(a) Prove that $G$ contains a [[Normal Subgroup|normal]] [[Sylow p-Subgroup|Sylow subgroup]].
(b) Suppose $p < q$ and the Sylow $p$-subgroup is [[Cyclic|cyclic]] and normal. Prove that $G$ is [[Abelian Group|abelian]].

##### *Proof.*
##### Part (a)
Let $G$ be a group of order $p^2q$ where $p$ and $q$ are distinct primes. Suppose by way of contradiction that $G$ has no normal Sylow $p$-subgroup. 

First, suppose $p<q$. By Sylow's Theorem we know the following:
- $n_p|q$ and $n_p\equiv 1\mod{p}$, so $n_p=1$ or $q$, so $q$
- $n_q|p^2$ and $n_q\equiv 1\mod{q}$, so $n_q=1$ or $p^2$, so $p^2$.
We know there must be $(q-1)\cdot p^2=p^2q-p^2$ elements of order $p$. Luckily, there is more than one Sylow $p$-subgroup with $p^2$ elements, so there isn't room for all of them.

Suppose then that $q>p$. By Sylow's Theorem we know the following:
- $n_p|q$ and $n_p\equiv 1\mod{p}$, so $n_p=1$, so we're definitely good there.
***
###### Part (b)
Suppose $p < q$ and the Sylow $p$-subgroup, $P$, is cyclic and normal. We know from Part (a) that there are either $1$ or $p^2$ Sylow $q$-subgroups, but since there are already $p^2$ elements of order $p$ there is only room for one, $Q$, which is also cyclic, given its prime power. As $P$ and $Q$ are thus normal in $G$ and only intersect trivially, we see that $PQ=G$, meaning that $G=P\times Q$. Thus $G$ is the product of two cyclic groups of relatively prime order, making $G$ cyclic as well. Cyclic groups are abelian, so we are done.
***

### Problem 3 – Group of Order $p^2q$
Let $G$ be a finite group of order $p^2q$ with $p < q$ prime numbers. Show that $G$ is not a simple group.

##### *Proof.*
Let $G$ be a finite group of order $p^2q$ with $p < q$ prime numbers, and suppose by way of contradiction that $G$ is simple. By Sylow's Theorem we have the following:
- $n_p|q$ and $n_p\cong 1\mod{p}$, and thus $n_p=q$. 
- $n_q|p^2$ and $n_q\cong 1\mod{q}$, and thus $n_q=p^2$. 
From this information we see that there are $p^2(q-1)$ elements of order $q$ and $(p^2-1)q$ elements of order $p$, for a lovely total of $p^2q-p^2+p^2q-q$ elements, which is too many.
***
#qual