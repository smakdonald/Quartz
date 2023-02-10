#### $\cor$ – Invariant Factors are Diagonal SNF Entries
The invariant factors of a matrix $A$ are the non-zero, non-unit diagonal entries of the [[Theorem – Smith Normal Form|Smith Normal Form]] of $xI_n - A$.

###### *Proof.* 
Let $S$ be the Smith Normal Form of $xI_n - A$ and let $d_1, \dots, d_n$ be its diagonal entries. As proven before, the matrix $xI_n - A$ and $S$ present isomorphic $F[x]$-modules, and thus the Theorem gives an isomorphism
$$
F^n_A \cong F[x]/(d_1) \oplus \cdots \oplus F[x]/(d_n).
$$
Since $\dim_F F^n_A < \infty$, none of the $d_i$'s can be zero. So, each $d_i$ is monic and $d_1 \mid \cdots \mid d_n$. Now some of the $d_i$ might be non-zero constants, in which case $d_i$ is a unit and $F[x]/(d_i) = 0$. Upon tossing those out, we are left with $$F^n_A \cong F[x]/(f_1) \oplus \cdots \oplus F[x]/(f_k)$$with each $f_i$ monic of positive degree and $f_1 \mid \cdots \mid f_k$. These are, by definition,  the invariant factors of $A$.
***