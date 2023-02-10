### Problem 10 – Field Extensions and Similar Transposes
Let $A$ and $B$ be $n\times n$ matrices with entries in $F$. Recall that $A$ and $B$ are said to be [[Similar Matrices|similar]] over $F$ if there exists an invertible $n\times n$ matrix, with entries in $F$, such that $B = P\inv AP$.
Prove the following statements about matrices $A$ and $B$ with entries in $F$:

(a) If $F \subseteq K$ is a [[Field Extension|field extension]], and $A$ and $B$ are similar over $K$, then they are similar over $F$.
(b) $A$ is similar over $F$ to its transpose $A^T$.

##### *Proof.*

###### Part (a) 
Suppose $A$ and $B$ are similar in $\Mat_{n \times n}(K)$. As $A$ and $B$ have entries in $F$, then they are both in $\Mat_{n \times n}(F)$. Thus there exist matrices $C,D\in\Mat_{n \times n}(F)$ in RCF such that $A$ is similar to $C$ and that $B$ is similar to $D$. However, $A$ is similar to $C$ and that $B$ is similar to $D$ in $\Mat_{n \times n}(K)$ as well. Notice $C$ and $D$ are still in RCF. However, as the RCF is unique, this means that $C=D$ in $\Mat_{n \times n}(K)$, making them equal in $\Mat_{n \times n}(F)$ as well. Thus $A$ is similar to $B$, as similarity is transitive.
***
###### Part (b) 
Let $L$ be the algebraic closure of $F$. Thus $A$ has a Jordan Canonical Form in $L$. For each Jordan block $J_i$ in the JCF of $A$, let $B_i$ denote the transpose of the identity matrix, and notice that $B_iJ_iB_i\inv=J_i^T$. As this is the case for every Jordan block, we see that the JCF of $A$, $J$, is similar to its transpose. As the $A$ is similar to $J$, $A^T$ is similar to $J^T$, and $J$ is similar to $J^T$, we see that $A\sim A^T$ in $L$ by transitivity. From Part (a), this yields $A\sim A^T$ in $F$. 
***
#qual