### Problem 6 – Similarity Classes and CharPoly
Determine all [[Similar Matrices|similarity]] [[Equivalence Class|classes]] of matrices with entries in $\Q$ with [[Characteristic Polynomial|characteristic polynomial]] $(x^4-1)(x^2-1)$. Provide an explicit representative for each of these similarity classes.

##### *Proof*.
Let $A$ be a matrix with entries in $\Q$ with characteristic polynomial $(x^4- 1)(x^2 -1)$.

By this [[Corollary – Every Matrix Similar to Unique RCF Matrix|Corollary]] we know that every matrix is similar to a unique matrix in RCF. Note that RCF is based on the invariant factors if a matrix, and thus if two matrices have the same invariant factors they will have the same RCF, making them both similar to the same (unique) matrix, making them similar to each other. By part (1) of this [[Theorem – Cayley-Hamilton Theorem|Theorem]], the characteristic polynomial of a matrix is equal to the product of the invariant factors of that same matrix. 

Recall that the invariant factors must divide all preceding invariant factors in RCF (See: [[Theorem – Rational Canonical Form|Theorem]]), and observe that $(x^4-1)$ factors as $(x^2-1)(x^2+1)$ and $(x^2-1)$ factors as $(x-1)(x+1)$. Given this information, after some fiddling with the factors, we find four possible options for invariant factors of $A$:
1. $x^6-x^4-x^2+1=(x^2 -1)(x^4- 1)$,
2. $(x^2-1),(x^4-1)$,
3. $(x+1), (x-1)(x^4-1)$, and 
4. $(x-1),(x+1)(x^4-1)$.
Let $f(x)=x^6-x^4-x^2+1, g(x)=(x^4-1),$ $h(x)=x^2-1$, $j(x)=(x-1),$ and $k(x)=(x+1)$.
Observe the companion matrices of each of these polynomials:
$$C(f)=\begin{bmatrix}
0 & 0 & 0 & 0 & 0 & -1\\
1 & 0 & 0 & 0 & 0 & 0\\
0 & 1 & 0 & 0 & 0 & 1\\
0 & 0 & 1 & 0 & 0 & 0\\
0 & 0 & 0 & 1 & 0 & 1\\
0 & 0 & 0 & 0 & 1 & 0\\
\end{bmatrix},
C(g)=\begin{bmatrix}
0 & 0 & 0 & 1\\
1 & 0 & 0 & 0\\
0 & 1 & 0 & 0\\
0 & 0 & 1 & 0\\
\end{bmatrix},
C(h)=\begin{bmatrix}
0 & 1\\
1 & 0\\
\end{bmatrix},
C(j)=\begin{bmatrix}
1\\ 
\end{bmatrix}\textrm{ and } 
C(k)=\begin{bmatrix}
-1\\ 
\end{bmatrix}
$$
Behold: explicit representatives of each similarity class:
1. $C(f)$,
2. $C(g)\oplus C(h)$,
3. $C(k)\oplus C(gj)$, and
4. $C(j)\oplus C(gk)$.
***
#qual