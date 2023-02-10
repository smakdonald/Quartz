#### $\cor$ – Every $m\times n$ Matrix Equivalent to Unique Matrix 
Every $m \times n$ matrix $A$ with entries in a [[Field|field]] is equivalent to a unique matrix of the form$$\begin{bmatrix}
I_r & 0 \\
0 & 0 \\
\end{bmatrix}$$
where $r$ is the rank of $A$. 

###### *Proof.* 
Let $V = F^n$ and $W = F^m$ and $g: V \to W$ be the  linear transformation given by $g(v) = A \cdot v$, matrix multiplication. (I have called this map $T_A$ in the past.) If $B'$ and $C'$ are the standard basis of $V$ and $W$ then $[g]_{B'}^{C'} = A$.
  
The Theorem gives that there are bases $B$ and $C$ of $V$ and $W$ such that$$[g]_B^C = 
 \begin{bmatrix}
I_r & 0 \\
0 & 0 \\
\end{bmatrix}.$$So, by Proposition \ref{prop:changebase}, we have
$$A = [g]_{B'}^{C'} = [\id_W]_C^{C'}[g]_B^C [\id_V]_{B'}^{B}=P
\begin{bmatrix}I_r & 0 \\0 & 0 \\\end{bmatrix}Q$$
with $P := [\id_W]_C^{C'}$ and $Q := [\id_V]_{B'}^{B}$. Note that $P, Q$ are invertible since they are change of basis matrices (see \eqref{E29}). 

The uniqueness of $r$ follows from the fact that $r = \rank_F(g)$, which does not depend on a choice of bases. 
***