#### $\defn$ – Multilinear and Alternating
For any [[Commutative Ring|commutative]] [[Ring|ring]] $R$ and $R$-[[Module|module]] $V$, given a function of the form $$\phi: \overbrace{V \times \cdots \times V}^n \to R$$ we say:
1. $\phi$ is $R$-*mutli-linear* if, for each $i$, we have $$\phi(v_1, \dots, v_{i-1}, v_i + v'_i, v_{i+1}, \dots, v_n) = \phi(v_1, \dots, v_{i-1}, v_i , v_{i+1}, \dots, v_n) +\phi(v_1, \dots, v_{i-1},  v_i', v_{i+1}, \dots, v_n)$$and $$\phi(v_1, \dots, v_{i-1}, r v_i, v_{i+1}, \dots, v_n) = r \phi(v_1, \dots, v_{i-1},  v_i, v_{i+1}, \dots, v_n) $$for all elements $v_1, \dots, v_n, v_i'$ in $V$ and all $r \in R$.
2. $\phi$ is *alternating* if $\phi(v_1, \dots, v_n) = 0$ if $v_i = v_j$ for some $i \ne j$. 
***