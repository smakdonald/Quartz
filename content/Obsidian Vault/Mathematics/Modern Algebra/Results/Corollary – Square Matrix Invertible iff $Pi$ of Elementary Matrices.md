#### $\cor$ – Square Matrix Invertible iff $\Pi$ of Elementary Matrices
If $F$ is a [[Field|field]], then a square matrix is invertible if and only if it is a product of [[Elementary Matrix|elementary matrices]].

###### *Proof.* 
($\Leftarrow$) Every elementary matrix is invertible and a product of invetible matrices is again invertible. 

($\Rightarrow$) If $A$ is invertible, then by the previous Corollary and Lemma \ref{lem219} there exists elementary matrices $E_1, \dots, E_s$, $F_1, \dots, F_t$ of type I or II such that $$E_s \cdots E_1 \cdot A \cdot F_1 \cdots F_t= I_n$$ and hence $A = E_1^{-1} \cdots E_s^{-1}F_t^{-1} \cdots F^{-1}_1$. This proves the statement since the inverse of an elementary matrix is an elementary matrix.
***