#### $\thm$ – Dimension and Subspaces
Let $F$ be a [[Field|field]] and let $W$ be a [[Submodule|subspace]] of a [[Dim (Vector Space)|finite dimensional]] $F$-[[Vector Space|vector space]] $V$. Then[^1] $$\dim(V) = \dim(W) + \dim(V/W).$$

###### *Proof.* 
Pick a basis $X$ of $W$. Regarded as a subset of $V$, $X$ remains linearly independent and thus it may be extended to a basis of $V$ by Corollary \ref{cor:basisexist}. Let us write this basis of $V$ as $X \cup Y$ with $X \cap Y = \emptyset$. 

Let $Z := \{y + W \mid y \in Y\} \subseteq V/W$. I claim that $Z$ is a basis of $V/W$.

Given $v + W$ we have $v = \sum_i a_i x_i + \sum_j b_j y_j$ for some $x_i \in X, y_j \in Y$ and scalars $a_i, b_j$. 
Since $x + V = 0$ for all $x \in X$, we have $v + W = \sum_j b_j z_j$. This proves $Z$ spans. Say $\sum_j c_j y_j + W = 0$ for some $y_1, \dots, y_m \in Y$. Then $\sum_j c_j y_j \in W$ and hence $\sum_j c_j y_j = \sum_i a_i x_i$, whence $\sum_j c_j y_j + \sum_i - a_i x_i = 0$. Since $X \cup Y$ is linearly independent, $c_j = 0$ and $a_i = 0$ for all $j, i$. This proves $Z$ is linearly independent.

We have $$\dim(V) = |X \cup Y| = |X| + |Y| = |X|+ |Z| = \dim(W) + \dim(V/W).$$with the second equality holding since $X$ and $Y$ are disjoint. 
***

[^1]: See: [[Dim (Vector Space)|Dimension]], [[Quotient Module]]