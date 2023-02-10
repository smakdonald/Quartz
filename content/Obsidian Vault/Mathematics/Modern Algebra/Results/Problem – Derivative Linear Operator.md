### Problem 6 – Derivative Linear Operator
Consider the $\C$-[[Vector Space|vector space]] $V = {p \in \C[x] : \deg(p) \leq n - 1}$. (You may assume without proof that $V$ is n-[[Dim (Vector Space)|dimensional]].) Consider the following [[Linear Operator|linear maps]] $V \to V$:  
$$D : V \to V \hspace{4cm} T : V \to V$$
$$p\mapsto p'\hspace{4cm} p\mapsto xp'$$
(where p′ denotes the [[Derivative|derivative]] of p). Determine the [[Theorem – Jordan Canonical Form|Jordan normal form]] of
(a) $D$
(b) $B$

##### *Proof*.

###### Part (a)
For any integer $n \geq 1$, consider the $\C$-vector space $V = \{p \in \C[x] : \deg(p) \leq n - 1\}$.

Let $T:V \to V$ be the linear operator given by $T(p) = xp'$ (where $p'$ denotes the derivative of $p$). Note that the [[Change of Basis Matrix|change of basis]] matrix for this operator is given by $$
\begin{bmatrix}
  0 & 0 & \cdots & 0 & 0 \\
  0 & 1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & n-1 \\   
\end{bmatrix},
$$
with the basis $\{1,x,\dots,x^{n-1}\}$. Thus $\cp_A(x)$ will be given by the [[Determinant|determinant]] of the matrix


$$
\begin{bmatrix}
  x & 0 & \cdots & 0 & 0 \\
  0 & x-1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & x-(n-1) \\   
\end{bmatrix},
$$

which is diagonal. Hence $$\cp_AT(x)=\displaystyle\prod_{i=0}^{n-1}(x-i).$$Thus $\cp_AT(x)$ factors into distinct linear polynomials, each of which is in the form $(x-i)$ for $0\leq i\leq n-1$. Thus each linear term is an elementary divisor, making each Jordan block a $1\times1$ matrix with $i$ as the only entry. Thus the Jordan Canonical form is $$\begin{bmatrix}
  0 & 0 & \cdots & 0 & 0 \\
  0 & 1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & n-1 \\   
\end{bmatrix}.
$$
***
###### Part (b)
This time around the change of basis matrix (denoted $B$ and using the same basis as above) for this matrix has 0s along the diagonal, and increasing natural numbers (starting at 0, sorry) along the upper diagonal. Thus $\cp_B(x)=x^n$.

Recall that the minimal polynomial corresponding to $B$ will be the the smallest monic polynomial such that $B$ is sent to 0. Note that as $D$ is the operator sending $p$ to its derivative, and that $D^{(2)}=D(D(p))=p''=p^{(2)}$. Thus $B^2$ can be viewed as a change of basis matrix for taking the second derivative of the basis, and so on.

As the basis extends to $x^{n-1}$, it requires $n$ derivatives to make this polynomial become 0. Thus the minimal polynomial of $B$ must be $x^n$, as it it monic and $B^n=0$. As the degree of the invariant factors must sum to $n$ and $\mp_B(x)=x^n$, which is itself an invariant factor, we see that it must in fact be the only one.

As $x^n$ is already a power of a prime, it is the only elementary divisor as well. Thus the Jordan Canonical Form for $B$ is an $n\times n$ Jordan Block with 0s along the diagonal and 1s along the sub-diagonal. 
***
#qual