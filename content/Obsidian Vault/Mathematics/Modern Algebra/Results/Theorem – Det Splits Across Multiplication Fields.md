#### $\thm$ – Det Splits Across Multiplication: Fields
For a [[Field|field]] $F$ and matrices $A, B \in \Mat_{n \times n}(F)$ we have[^1] $$\det(AB) = \det(A)\det(B).$$
###### *Proof.* 
If $A$ is not invertible, neither is $AB$, since $\im(AB) \subseteq \im(A)$, and if $B$ is not invertible, neither is is $AB$, since $\ker(AB) \supseteq \ker(A)$. So, by Corollary \ref{cor227b}, if either $A$ or $B$ is not invertible, both sides of the equation are $0$.

Assume now that $A$ and $B$ are both invertible.  Then by Corollary \ref{cor220} we have $$
A = E_1 \cdots E_n$$and$$
B = F_1 \cdots F_m
$$and hence
$$
AB = E_1 \cdots E_n F_1 \cdots F_m
$$where the $E_i$'s and $F_j$'s are elementary matrices. Applying Corollary \ref{cor220} repeatedly gives $$
\det(AB) = \det(E_1 \cdots E_n F_1 \cdots F_{m-1}) \det(F_m) = \cdots
= \det(E_1) \cdots \det(E_n) \det(F_1) \cdots \det(F_m)$$and similarly$$
\det(A) \det(B) = \left(\det(E_1) \cdots \det(E_n)\right) \left( \det(F_1) \cdots \det(F_m)\right).
$$
***

[^1]: See: [[Determinant]]