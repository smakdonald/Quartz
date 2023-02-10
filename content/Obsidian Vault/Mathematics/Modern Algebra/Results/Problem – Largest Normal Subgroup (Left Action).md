### Problem 1 – Largest Normal Subgroup (Left Action)
Let $G$ be a (not necessarily [[Order|finite]]) [[Group|group]] and $K \leq G$ a [[Subgroup|subgroup]] of [[Index|index]] $n < \infty$. Define
$$N=\bigcap_{g\in G}gKg\inv$$(i.e., $N$ is the intersection of all the conjugates of K$)$

(a) Prove $N$ is a the largest [[Normal Subgroup|normal subgroup]] of $G$ that is contained in $K$.
(b) Prove $[G : N ]$ divides $n!$.

##### *Proof.*
###### Part (a)
Let $G$ act on the left cosets of $K$ in $G$ by left multiplication, yielding the permutation representation homomorphism $\rho:G\to S_n$. Let $N$ conspicuously denote the kernel of this function. 

Let $x\in N$. Then $\rho(n)$, the automorphism $\s:G/K\to G/K$ defined by $\s(gK)=xgK$ is precisely the identity permutation. Thus $xgK=gK$ for all $g\in G$ and $g\inv xgK=K$ for all $g\in G$, so $x\in$ This means the elements of $N$ are precisely those that are in the conjugacy class of $gKg\inv$ for all $g\in G$. There cannot exist a larger normal subgroup of $G$ contained in $K$, as it would contain an element that was not in some conjugacy class for $G$, negating the definition of a normal subgroup. 
***
###### Part (b)
Recall the permutation representation homomorphism $\rho:G\to S_n$. The First Isomorphism Theorem tells us $G/N\cong\im(\rho)\leq S_n$, which has order $n!$. Thus $[G:N]|n!$. 
***
#qual