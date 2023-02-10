### Problem 7 – January 2014 (9)
Let $F$ be a field and $A$ a square matrix with entries from $F$. Prove that $A$  
is similar to its transpose.

##### *Proof*.
Let $L$ be the algebraic closure of $F$. Thus $A$ has a Jordan Canonical Form in $L$. For each Jordan block $J_i$ in the JCF of $A$, let $B_i$ denote the transpose of the identity matrix, and notice that $B_iJ_iB_i\inv=J_i^T$. As this is the case for every Jordan block, we see that the JCF of $A$, $J$, is similar to its transpose. As the $A$ is similar to $J$, $A^T$ is similar to $J^T$, and $J$ is similar to $J^T$, we see that $A\sim A^T$ in $L$ by transitivity. 

Suppose $A$ and $B$ are similar in $\Mat_{n \times n}(L)$. As $A$ and $B$ have entries in $F$, then they are both in $\Mat_{n \times n}(F)$. Thus there exist matrices $C,D\in\Mat_{n \times n}(F)$ in RCF such that $A$ is similar to $C$ and that $B$ is similar to $D$. However, $A$ is similar to $C$ and that $B$ is similar to $D$ in $\Mat_{n \times n}(L)$ as well. Notice $C$ and $D$ are still in RCF. However, as the RCF is unique, this means that $C=D$ in $\Mat_{n \times n}(L)$, making them equal in $\Mat_{n \times n}(F)$ as well. Thus $A$ is similar to $B$, as similarity is transitive.

This yields $A\sim A^T$ in $F$. 
***
#qual