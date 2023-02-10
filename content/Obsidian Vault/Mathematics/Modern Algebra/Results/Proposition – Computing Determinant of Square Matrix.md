#### $\prop$ – Computing Determinant of Square Matrix
Let $R$ be any non-zero [[Commutative Ring|commutative]] [[Ring|ring]]. Let $A$ be a square matrix and let $B$ be a matrix obtained form $A$ by a single elementary column operation: #fix 
1. If the operation is of type I, $\det(B) = \det(A)$[^1].
2. If the operation is of type II, given by multiplying a column of $A$ by a [[Unit|unit]] $u$, then $\det(B)=u\det(A)$.
3. If the operation is of type III, $\det(B)=-\det(A)$.
  
###### *Proof.* 
The first claim follows from  multi-linearity and alternating properties: For notational simplicity say $A = (v_1, v_2, \dots)$ and $B = (v_1 + rv_2, v_2, \dots)$. Then$$
  \det(B) = \det(v_1, v_2, \dots) + r \det(v_2, v_2, \dots) = \det(A) + r \cdot 0 = \det(A)
  $$The second is immediate from (the second part of) $R$-multi-linearity. The last is a special case of Lemma \ref{lem221}. 
***

[^1]: See: [[Determinant]]