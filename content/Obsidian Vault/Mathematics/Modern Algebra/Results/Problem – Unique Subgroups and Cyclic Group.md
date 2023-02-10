### Problem 2 – Unique Subgroups and Cyclic Group

Suppose $G$ is a [[Order|finite]] [[Group|group]] which has precisely one [[Subgroup|subgroup]] of [[Order|order]] $d$ for each divisor $d$ of $|G|$. Prove that $G$ is [[Cyclic|cyclic]].

##### *Proof.*
First, suppose that $G$ is a $p$-group. Let $g\in G$ have biggest order. Let $h\in G$. So $|h|\bigg||g|$. Since $(g)\leq G$, it also has exactly one subgroup for each divisor. But (h) has the same order as one of those subgroups, so they must be the same group. So $h\in(g)$. Since $h$ was arbitrary, then $G\leq (g)$. So when $G$ is a $p$-group then it is cyclic. 

If its not a $p$-group then we can decompose $|G|$ into relatively prime powers of primes, all of which are $p$-groups and maintain this property. Thus $G$ is the product of relatively prime cyclic groups, making it cyclic itself. 
***
#qual