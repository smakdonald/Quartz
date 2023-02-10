#### $\prop$ – Matrix Invertible iff Det is a Unit
For any non-zero [[Commutative Ring|commutative]] [[Ring|ring]] $R$ and any $A \in \Mat_{n \times n}(R)$, $A$ is invertible if and only if $\det(A)$[^1] is a [[Unit|unit]] of $R$. 

###### *Proof.* 
If $A$ is invertible then $1 = \det(I_n) = \det(AA^{-1}) = \det(A) \det(A^{-1})$ by the Theorem, and hence $\det(A)$ is a unit. 

If $\det(A)$ is a unit, then, using the equation above, we have
$$
A (A^{adj} \cdot \frac{1}{\det(A)}) =I_n = (A^{adj} \cdot \frac{1}{\det(A)}) A
$$
which proves $A$ has a two-sided inverse (namely, $A^{adj} \frac{1}{\det(A)}$). 
***

[^1]: See: [[Determinant]]