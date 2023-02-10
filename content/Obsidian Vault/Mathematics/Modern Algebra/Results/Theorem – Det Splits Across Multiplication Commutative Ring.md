#### $\thm$ – Det Splits Across Multiplication: Commutative Ring
For any non-zero [[Commutative Ring|commutative]] [[Ring|ring]] $R$  and matrices $A, B \in \Mat_{n \times n}(R)$, we have[^1] $$\det(AB) = \det(A) \det(B) \in R. $$

###### *Proof.* 
We have already proven that this holds when $R$ is a field.

We next show that it holds whenever $R$ is an integral domain. In this case, $R$ is a subring of a field $F$ (namely, the field of fractions of $R$). So, we know that  the equation $\det(AB) = \det(A) \det(B)$  holds in $F$ if we interpret $A$ and $B$ as belonging to $\Mat_{n \times n}(F)$. But the value of $\det$ is the same if we interpret these matrices as having entries in $R$ or in $F$. So $\det(AB) = \det(A) \det(B)$ holds in $R$. 

We finally prove that the Theorem for any non-zero commutative ring $R$ by building on the fact  that it holds for domains.  We do so by contructing a ring homomorphism $g: S \to R$ and
matrices $X$ and $Y$ in $\Mat_{n \times n}(S)$ such that $S$ is an integral domain, $g(X) = A$ and $g(Y) = B$. Granting such a $S, g, X$ and $Y$ exist, the result follows from the naturality of $\det$ (Lemma \ref{lem220}). In detail, we know $\det(XY) = \det(X) \det(Y)$, since $S$ is a domain.
Since the rule for multiplying matrices involves only sums and products of ring elements, we have $g(XY) = g(X)g(Y)$.   So$$
\begin{aligned}
  \det(AB) & = \det(g(X) g(Y)) 
   = \det(g(XY))  = g \det(XY) \\ 
   & = g(\det(X) \det(Y)) = g(\det(X)) g(\det(Y)) = \det(g(X)) \det(g(Y)) = \det(A) \det(B).
 \end{aligned}$$It remains to prove such a $S$, $g$, $X$ and $Y$ exists.  Suppose $A = (a_{i,j})$ and $B = (b_{i,j})$. 
Form the polynomial ring$$
  S := \Z[\{x_{i,j} \mid 1 \leq i \leq n, 1 \leq j \leq n\} \cup \{y_{i,j}\mid 1 \leq i \leq n, 1 \leq j \leq n\}]
  $$of $2 n^2$ variables with $\Z$-coefficients. By the UMP for polynomial rings with integer coefficients, since $R$ is commutative, there is a (unique) ring map $g: S \to R$ such that $g(x_{i,j}) = a_{i,j}$ and $g(y_{i,j}) = b_{i,j}$ for all $i,j$. That is, $g$ is the evaluation map given by setting $x_{i,j} = a_{i,j}$ and $y_{i,j} = b_{i,j}$ for all $i,j$, and interpreting integers as elements of $R$. Let $$X = (x_{i,j}), Y = (y_{i,j})  \in \Mat_{n \times n}(S)$$ be the evident matrices of indeterminants.Then $S$ is a domain, $g: S \to R$ is a ring homomorphism, $g(X) = A$ and $g(Y) = B$, as desired.
***

[^1]: See: [[Determinant]]