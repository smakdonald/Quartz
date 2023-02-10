### Problem 6 – JCF and RCF of Derivative Operator
Let $n$ be a positive integer. Consider the real [[Vector Space|vector space]] $V = \{p \in R[x] | \deg(p) \leq n\}$  and the [[Linear Transformation|linear transformation]] $T : V \to V, T (p) = p'$, where $p'(x)$ is the [[Derivative|derivative]] of p(x).

(a) Find the [[Characteristic Polynomial|characteristic polynomial]] and the [[Minimum Polynomial|minimal polynomial]] for $T$.
(b) Find the [[Invariant Factor|invariant factors]] and the [[Elementary Divisor|elementary divisors]] for $T$.
(c) Find the [[Theorem – Rational Canonical Form|rational canonical form]] and the [[Theorem – Jordan Canonical Form|Jordan canonical form]] for $T$.

##### *Proof.*
Let $T:V \to V$ be the linear operator given by $T(p) = xp'$ (where $p'$ denotes the derivative of $p).$

###### Part (a)
Note that the change of basis matrix for this operator is given by $$
\begin{bmatrix}
  0 & 0 & \cdots & 0 & 0 \\
  0 & 1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & n-1 \\   
\end{bmatrix},
$$
with the basis $\{1,x,\dots,x^{n-1}\}$. Thus $\cp_A(x)$ will be given by the determinant of the matrix $$\begin{bmatrix}
  x & 0 & \cdots & 0 & 0 \\
  0 & x-1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & x-(n-1) \\   
\end{bmatrix},$$
which is diagonal. Hence $\cp_AT(x)=\displaystyle\prod_{i=0}^{n-1}(x-i)$.
***
###### Part (b)
Our $\cp_AT(x)$ factors into distinct linear polynomials, each of which is in the form $(x-i)^1$ for $0\leq i\leq n-1$. Thus each linear term is an elementary divisor. However, as none of these elementary divisors divide any of the others, we see that the only invariant factor is $\cp_AT(x)$ itself. 
***
###### Part (c)
As each linear term is an elementary divisor, each Jordan block a $1\times1$ matrix with $i$ as the only entry. Thus the Jordan Canonical form is $$\begin{bmatrix}
  0 & 0 & \cdots & 0 & 0 \\
  0 & 1 & \cdots & 0 & 0 \\
  \vdots & \vdots & \ddots & \vdots & \vdots \\
  0 & 0 & \cdots & 0 & n-1 \\   
\end{bmatrix}.$$
As the only invariant factor is $\cp_AT(x)$, we see that the Rational Canonical Form of $T$ is $C(\cp_AT(x))$.
***
#qual