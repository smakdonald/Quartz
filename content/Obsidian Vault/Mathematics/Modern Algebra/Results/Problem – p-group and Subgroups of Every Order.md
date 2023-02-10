### Problem 2 – $p$-group and Subgroups of Every Order
Let $G$ be a [[Group|group]] of [[Order|order]] $p^n$[^1] where $p$ is a prime and $n \geq 1$.

(a) Prove the [[Center|center]] of G is not trivial.
(b) Prove there exists a [[Subgroup|subgroup]] of order $p^j$ for each $j$ satisfying $0 \leq j \leq n.$

##### *Proof.*
Let $G$ be a group of order $p^n$ where $p$ is a prime and $n \geq 1$.

##### Part (a)
The [[Theorem – The Class Equation|Class Equation]] tells us[^2]
$$|G|=|Z(G)|+\sum\limits_{g\in G}[G:C_G(g)],$$where $C_G(g)$ are the [[Centralizer & Normalizer|centralizers]] with more than one element. Notice that this means $|C_G(g)|\big||G|$, and thus each centralizer is a power of $p$. Thus we have $$p^n=|Z(G)|+pk$$for some $k\in\N$. Thus the center of $G$ cannot be trivial, else we would not be able to sum to a power of $p$. 
***
###### Part (b)
The trivial subgroup has order $1=p^0$. Suppose inductively that there exists a subgroup of order $p^{j}$ that has a subgroup for every power of $p$ in between. 

Consider, if you will, a group of order $p^{j+1}$, $H$. As this is a $p$-group, by Part (a) the center is nontrivial, making it a $p$ group as well, and thus it has a subgroup of order $p$, $K$, which is normal in $H$ as it lies within the center, so we mod out by $K$ to see that $H$ has a subgroup of order $p^j$, which has subgroups of all the other powers by the induction hypothesis. 
***
#qual

[^1]: Note that this makes $G$ a $p$-[[p-group|group]].
[^2]: Notation: [[Index]], [[Center]], 