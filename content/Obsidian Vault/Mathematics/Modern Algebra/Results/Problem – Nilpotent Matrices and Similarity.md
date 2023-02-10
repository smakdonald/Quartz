### Problem 7 – Nilpotent Matrices and Similarity
Let $F$ be a [[Field|field]] and recall that a square matrix $A$ with entries in $F$ is called [[Nilpotent|nilpotent]] if $A^m = 0$ for some positive integer $m$.

(a) Prove that if $A$ is an $n \times n$ nilpotent matrix, then $A^n = 0$.
(b) Assume $n \leq 3$ and prove that two $n \times n$ nilpotent matrices are [[Similar Matrices|similar]] if and only if they have the same [[Rank|rank]]. (Recall the rank of a matrix is the [[Dim (Vector Space)|dimension]] of the [[Vector Space|vector space]] spanned by its columns.)
(c) Give an example, with justification, of two $4 \times 4$ nilpotent matrices that have the same rank but are not similar.

##### *Proof*.
Let $F$ be a field.

###### Part (a)
Let $A$ be an $n \times n$ nilpotent matrix. Let $\lambda$ be some eigenvalue of $A$. Thus there exists some vector $v$ such that $A\lambda=\lambda v$. Let's consider this the base-case of some rather banal induction. Now assume that for $n$ we have $A^nv=\lambda^nv$. Consider $$A^{n+1}v=A(A^nv)=A(\lambda^n v)=\lambda^n(Av)=\lambda^{n+1}v.$$Recall that as $A$ is nilpotent, there exists some $m\in\N$ such that $A^m=0$. As $\lambda$ is an eigenvalue of $A$, by the above induction we see that $\lambda^m$ is an eigenvalue for $A^m=0$. As $F$ is a field and thus an integral domain, we see that $\lambda^n=0$ implies that $\lambda=0$ is as well. As this holds in the algebraic closure of $F$ as well, we see that when factored into linear terms all the $\lambda=0$. Thus $\cp_A(x)=x^n$. 

By the Cayley Hamilton Theorem we know $\mp_A(x)|\cp_A(x)=x^n$, and thus $A^n=0$. 
***
###### Part (b)
Assume $n \leq 3$ and let $A,B$ be nilpotent matrices with entries in $F$.

$(\Rightarrow)$ Suppose $A\sim B$. Thus there exists some invertible matrix $P$ such that $PAP\inv=B$ by the definition of [[Definitions#Similar Matrices|similar matrices]]. Let $U\in\ker(PA)$. Thus $PA(U)=0$ and $P(AU)=0$. We multiply both sides by $P\inv$ to see that $AU=0$. Therefore the $\ker(PA)=\ker(A)$, and hence the ranks of $PA$ and $A$ are equal by the [[Results#Corollary – Rank Nullity Theorem|Rank-Nullity Theorem]]. 

Next, observe $$\begin{align}
    \rank(AP\inv)&=\rank((AP\inv)^T)\\
    &=\rank(P^{-1^T}A^T)\\
    &=\rank(A^T)\\
    &=\rank(A),
\end{align}$$as $(P^{-1})^T$ is an invertible matrix. Thus $\rank(B)=\rank(PAP\inv)=\rank(A)$.

$(\Leftarrow)$ Suppose that $\rank(A)=\rank(B)$. From Part (a) we know $\cp_A(x)=\cp_B(x)=x^n$. 

We consider the case where $\cp_A(x)=\cp_B(x)=x^3$.

The only possible invariant factors involving $x^3$ are 
1. $x,x,x$;
2. $x,x^2$; and 
3. $x^3$ itself.
However, if $x,x,x$ are the invariant factors then the rank of $A$ would be 3, making it invertible, contradicting the fact that 0 is an eigenvalue of $A$. Thus we need only consider the latter two cases.

Note that $$C(x)=[0], C(x^2)=
\begin{bmatrix}
0 & 0\\
1 & 0\\
\end{bmatrix}, 
C(x)\oplus C(x^2)\begin{bmatrix}
0 & 0 & 0\\
0 & 0 & 0\\
0 & 1 & 0\\
\end{bmatrix}, \textrm{ and } C(x^3)=
\begin{bmatrix}
0 & 0 & 0\\
1 & 0 & 0\\
0 & 1 & 0\\
\end{bmatrix}.$$
As $C(x)\oplus C(x^2)$ has rank 1 and $C(x^3)$ has rank 2, since $\rank(A)=\rank(B)$ we see that they must have the same invariant factors, making them similar. 

If $n=2$ then the only possible invariant factor is $x^2$, as having two $x$'s would make $A$ and $B$ invertible again. If $n=1$ then $A=B=0$ and we're done. 
***
###### Part (c)
Consider $A=C(x^2)\oplus C(x^2)$ and $B=C(x)\oplus C(x^3)$.

Thus 
$$A=\begin{bmatrix}
0 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
0 & 0 & 0 & 0\\
0 & 0 & 1 & 0\\
\end{bmatrix} \textrm{ and } 
B=\begin{bmatrix}
0 & 0 & 0 & 0\\
0 & 0 & 0 & 0\\
0 & 1 & 0 & 0\\
0 & 0 & 1 & 0\\
\end{bmatrix},$$

both of which have rank $2$ and are in RCF. Thus they are not similar. 
***
#qual