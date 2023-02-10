#### $\thm$ – Gauss
Let $F$ be a [[Field|field]] and let $A$ be an $n \times n$ invertible matrix for $n \geq 1$. Then $A$ can be transformed to a matrix of the form $$ \begin{bmatrix}
     u & 0 & 0 & \cdots & 0 \\
     0 & 1 & 0 & \cdots & 0 \\
     0 & 0 & \ddots & \cdots & 0 \\
     \vdots & & \ddots & \ddots & \vdots  \\
     0 & 0 & \cdots & 0 & 1 \\
\end{bmatrix}$$ for some $u \ne 0$ via elementary [[Elementary Row & Column Operations|row]] and column operations of type I. 

###### *Proof.* 
Proceed by induction on $n$. If $n = 1$, there is nothing to prove (since $A$ cannot be the $0$ matrix.)  Assume $n > 1$ and that the result holds for $n-1$ by $n-1$ invertible matrices.

Let $A = (a_{i,j})$. Since $A$ is invertible, its column space must have dimension $n$, by the previous Lemma, and in particular none of its columns can be $0$ (since otherwise the column space would
be spanned by $n-1$ vectors and would thus have dimension at most $n-1$). In particular, its second-to-last column has at least one non-zero entry. By either doing nothing or by adding a suitable row to the last row, we can assume $a_{n,n-1} \ne 0$. By adding $(1 -a_{n,n}) a_{n,n-1}^{-1}$ times
column $n-1$ to column $n$, we obtain $a_{n,n} = 1$. Next do suitable column operations of type I to arrive at $a_{n,j} = 0$ for all $j < n$, and finally do row operations of type I to also get $a_{i,n} = 0$ for all $i < n$. We have thus transformed $A$ to a matrix of the form $\begin{bmatrix} A' & 0 \\ 0 & 1 \end{bmatrix}$.
Note that this matrix remains invertible (see Remark \ref{rem214}) and so the columns of this matrix span $F^n$ by the previous Lemma. Since $a_{n,j} = 0$ for all $j < n$,   the columns of $A'$ must span $F^{n-1}$. Thus $A'$ is invertible by the previous Lemma. By induction, we can transform $A'$ via type I row and column operations to a matrix of the form as in the statement. Notice that since the $a_{n,j} = 0$ for all $j < n$ and $a_{i,n} = 0$ for all $i < n$, such operations will also put $A$ into this form.
***