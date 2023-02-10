#### $\thm$ – Module Finite Implies Integral
Let $A\subseteq R$ be [[Module Finite|module-finite]]. Then $R$ is [[Integral Element|integral]] over $A$.

##### *Proof.*
Given $r\in R$, we want to show that $r$ is integral over $A$. The idea is to show that multiplication by $r$, realized as a [[Linear Transformation|linear transformation]] over $A$, satisfies the [[Characteristic Polynomial|characteristic polynomial]] of that linear transformation.

Suppose that $R = A f_1 + \cdots + A f_n$. We may assume that $f_1=1$, perhaps by adding a module generator. Since every element in $R$ is an $A$-[[Linear Combination|linear combination]] of $f_1, \ldots, f_n$, this is in particular true for the elements $rf_1, \ldots, r f_n$. Thus we can find $a_{ij} \in A$ such that $$r f_i = \sum_{j=1}^t a_{ij} f_j$$for each $i$. Consider the matrix $C=[a_{ij}]$ and the column vector $v=(f_1,\dots,f_n)$. We can now write the equalities above more compactly as $r  v = C v$. By the [[Lemma – Determinantal Technique|Determinantal Technique]], $\det(r I_{n\times n} - C)v=0$[^1]. Since we chose one of the entries of $v$ to be $1$, we have in particular that $\det(r I_{n\times n} - C)=0$. Expanding this [[Determinant|determinant]] as a polynomial in $r$, this is a monic equation with coefficients in $A$.

[^1]: Notation: [[Determinant]]