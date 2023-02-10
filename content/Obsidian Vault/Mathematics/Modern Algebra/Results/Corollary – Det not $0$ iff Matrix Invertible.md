#### $\cor$ – Det not $0$ iff Matrix Invertible
For $R = F$ a [[Field|field]], we have $\det(A) \ne 0$ if and only if $A$ is invertible.

###### *Proof.* 
If $A$ is not invertible, then the column space of $A$ is a proper subspace of $F^n$ and hence
the columns of $A$ must be linearly dependent. Say the $i$-th column is a linear combination of the rest: $v_i = \sum_{j \ne i} c_j v_j$. Then $$
\det(v_1, \dots, v_n) = \sum_{j \ne i} c_j \det(\text{a matrix with the $i$-th and $j$-th columns equal}) = 0.
$$If $A$ is invertible, then by Corollary \ref{cor217} $A$ can be obtained from $I_n$ via a sequence of elementary column operations. The result thus follows from Proposition \ref{prop227a} and the fact that $\det(I_n) = 1$. 
***