### Problem 1 – June 2012 (3)
Let $G$ be a [[Order|finite]] $p$-[[p-group|group]] for some prime $p$ and $N\neq {1}$ a [[Normal Subgroup|normal]] [[Subgroup|subgroup]] of $G$. Prove that $N\cap Z(G)\neq{1}$, where $Z(G)$ is the [[Center|center]] of $G$.

##### *Proof.*
Let $G$ be a finite $p$-group for some prime $p$ and $N\neq {1}$ a normal subgroup of $G$. 

First, we show that the center of $G$ is nontrivial. (See: [[Corollary – Center of $p$-group is Nontrivial|Corollary]]) Suppose by way of contradiction that $Z(G)=\{e\}$. We examine the [[Conjugacy Class|conjugacy classes]] of $G$. From the [[Theorem – The Class Equation|Class Equation]], we know$$|G| = |Z(G)| + \sum_i^r |G : C_G(g_i)|.$$Note that $|G|=p^n$ for some $n\in\N$, meaning that the only divisors of $|G|$ are powers of $p$. In finite groups, each conjugacy class must [[Corollary – $C_G(g_i) big G$ for Finite Groups|divide]] the order of the group. By [[Theorem – Lagrange's Theorem|Lagrange's Theorem]],  $|G : C_G(g_i)|=\frac{|G|}{|C_G(g_i)|}=\frac{p^n}{p^m}=p^k$, where $m,k\in\N$.  Since |Z(G)|=1, we see that $\sum_i^r |G : C_G(g_i)|\bigg|p^n-1$, which is impossible given that $p^{n-1} \not\mid p^n$. Thus $Z(G)\neq\{e\}$.

As $N\nsg G$ it is a [[Corollary – Normal Subgroups and Conjugacy Classes|union]] of conjugacy classes of the elements it contains, one of which is $e$. Assume by way of contradiction that $N\cap Z(G)={e}$, meaning that $e$ is the only element in $N$ whose conjugacy class is a singleton. This yields
$$|N| = 1+ \sum_i^r |G : C_G(g_i)|.$$
However, by Lagrange's Theorem $N$ must also be a $p-$group, and thus by an analogous element counting argument as above we see that there exists some $x\in N$ such that $C_G(x)=\{x\}$, or that $gxg\inv=x$ for all $g\in G$. Thankfully, this means that $x\in Z(G)$, and thus we have $Z(G)\cap N\neq 1$. 
#qual