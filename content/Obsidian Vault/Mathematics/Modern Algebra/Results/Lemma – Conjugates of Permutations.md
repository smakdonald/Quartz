#### $\lem$ – Conjugates of Permutations
For $\s \in S_n$[^1] and distinct integers $i_1, \dots, i_p$ we have
$$\s (i_1 \, i_2 \, \cdots i_p) \s^{-1} = (\s(i_1) \, \cdots \, \s(i_p)).$$
(Note that the right-hand [[Cycle|cycle]] is a cycle since $\s$ is one-to-one.)

###### *Proof.* 
To prove this, evaluate both sides at $\s(i_t)$ for any $t$ and observe that one gets $\s(i_{t+1})$ (with the supscript taken modulo $p$) both times. This proves they agree on the set $\s(\{i_1, \dots, i_p\})$. If $j$ is not in this set, then $(i_1 \, i_2 \, \cdots i_p)$ fixes $\sigma^{-1}(j)$ so the  left-hand side fixes $j$. So does the right, since $\s^{-1}(j) \notin \{\s(i_1), \dots, \s(i_p)\}$. Thus the two functions coincide on elements.
***

[^1]: See: [[Permutation Group]]