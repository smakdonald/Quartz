#### $\cor$ – Det Splits Across Elementary Multiplication
For any [[Commutative Ring|commutative]] [[Ring|ring]] $R$, if $A$ is an $n \times n$ matrix and $E$ is an $n \times n$ [[Elementary Matrix|elementary matrix]], then $$\det(AE) = \det(A) \det(E)$$

###### *Proof.* 
This follows from the Proposition and the fact that $AE$ is the result of doing the corresponding
column operation on $A$ (see Lemma \ref{lem219}), since $$
  \det(E)  = \begin{cases}
    1 & \text{if $E$ is elementary of type I} \\
    u & \text{if $E$ is elementary of type II with a unit $u$ on the diagonal} \\
    -1 & \text{if $E$ is elementary of type III.} \\
  \end{cases}$$These formulas follow from the formula for the determinant of an upper or lower triangular matrix --- see Example \ref{ex215}.
***