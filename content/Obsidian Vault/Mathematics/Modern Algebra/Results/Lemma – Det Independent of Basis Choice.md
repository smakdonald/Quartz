#### $\lem$ – Det Independent of Basis Choice
The [[Determinant|definition]] of $\det(\a)$ is independent of choice of $B$.

###### *Proof.* 
If $C$ is another basis, then 
$$
[\a]_C^C = P [\a]_B^B P^{-1}
$$
for an invertible matrix $P$ (specifically, $P = [\id]_B^C$). Then
$$
\det([\a]_C^C)  = \det(P [\a]_B^B P^{-1}) = \det(P) \det([\a]_B^B) \det(P^{-1}) =\det(P) \det(P^{-1}) \det([\a]_B^B) 
$$
using the Theorem. Also by the Theorem $\det(P) \det(P^{-1}) = \det(PP^{-1}) = \det(I_n) = 1$. 
***