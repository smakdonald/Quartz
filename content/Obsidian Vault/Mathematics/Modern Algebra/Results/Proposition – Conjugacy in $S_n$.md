#### $\prop$ – Conjugacy in $S_n$
Two elements of $S_n$[^1] are [[Conjugacy Class|conjugate]] if and only if they have the same [[Cycle|cycle]] type.

###### *Proof.* 
If two elements of $S_n$ are conjugate, say $\beta = \s \alpha \s^{-1}$, then they have the same cycle type, since we may write $\alpha$ as a product of disjoint cycles $\alpha = \alpha_1 \cdots \alpha_m$ and then apply this [[Lemma – Conjugates of Permutations|Lemma]]. Indeed, $\s \alpha \s^{-1} = (\s \alpha_1 \s^{-1})  \cdots (\s \alpha_m \s^{-1})$ and the Lemma shows that the right-side is a product of disjoint cycles.

Conversely, suppose $\alpha = \alpha_1 \cdots \alpha_k$ and $\beta = \beta_1 \cdots \beta_k$ are decompositions into disjoint cycles and that
$\alpha_i, \beta_i$ both have length $p_i \geq 2$ for all $i$. We need to prove $\alpha$ and $\beta$ are
conjugate. Let's start with the case $k = 1$: given two cycles of the same length
$$
\alpha = (i_1 \, \dots \, i_p) \text{ and } \beta = (j_1 \, \dots \, j_p).
$$
If $\s$ is any permutation such that $\s(i_m) = j_m$ for all $m = 1, \dots, p$, then $\s \a \s^{-1} = \beta$ by the Lemma. 

Note that such $\s$ is "allowed'' to map $\{1, \dots, n\} \setminus \{i_1 \, \dots \, i_p\}$ bijectively to $\{1, \dots, \} \setminus \{j_1 \, \dots \, j_p\}$ in any way possible. From this observation the general case follows: since the cycles are disjoint, we can find a single permutation $\s$ such that $\s \alpha_i \s^{-1} = \beta_i$ for all $i$.
***

[^1]: See: [[Permutation Group]]