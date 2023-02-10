### Problem 4 – JCF and Similarity
Let $A$ be the matrix with entries in $\C$
$$A=\begin{bmatrix}
3 & 0 & 0 & 0\\
1 & 3 & 0 & 0\\
1 & 0 & 3 & 0\\
0 & 2 & 1 & 3\\
\end{bmatrix}$$
(a) Find the [[Theorem – Jordan Canonical Form|Jordan canonical form]] of A.
(b) Is $A$ [[Similar Matrices|similar]] to
$$\begin{bmatrix}
0 & -9 & 0 & 0\\
1 & 6 & 0 & 0\\
0 & 0 & 0 & -9\\
0 & 0 & 1& 6\\
\end{bmatrix}?$$

##### *Proof.*
###### Part (a) 
First, notice that $A$ is upwards triangular, and thus $\cp_A(x)=(x-3)^4$. (See: [[Mathematics/Modern Algebra/Examples & Exercises#Example – Triangular Matrix and CharPoly|Example]]).  By the [[Results#Theorem – Cayley-Hamilton Theorem|Cayley-Hamilton Theorem]] the [[Minimum Polynomial|minimum polynomial]] divides the [[Characteristic Polynomial|characteristic polynomial]], and from the definition of minimum polynomial we know $\mp_A(x)$ is the smallest polynomial such that $\mp_A(A) = 0$. Since $\mp_A(x)$ must be a power of $(x-3)^n$ with $n\leq 4$, we plug in values of $n$ until we get $0$. 
$$(A-3I)^1=\begin{bmatrix}
0 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
0 & 2 & 1 & 0\\
\end{bmatrix}$$
Shucks. Moving on,
$$(A-3I)^2=\begin{bmatrix}
0 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
0 & 2 & 1 & 0\\
\end{bmatrix}\cdot\begin{bmatrix}
0 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
1 & 0 & 0 & 0\\
0 & 2 & 1 & 0\\
\end{bmatrix}=\begin{bmatrix}
0 & 0 & 0 & 0\\
0 & 0 & 0 & 0\\
0 & 0 & 0 & 0\\
3 & 0 & 0 & 0\\
\end{bmatrix},$$which is also not $0$. However, multiplying one more time we see $\mp_A(x)=(x-3)^3$. By part (2) of this [[Results#Theorem – Cayley-Hamilton Theorem|theorem]] $(x-3)^3$ is an [[Invariant Factors|invariant factor]]. By part (1) of that same theorem, invariant factors must multiply to $\cp_A(x)$, and so the invariant factors are $x-3$ and $(x-3)^3$. These are also the [[Elementary Divisors|elementary divisors]]. So 

$$J_1(3)\oplus J_3(3)=\begin{bmatrix}
3 & 0 & 0 & 0\\
0 & 3 & 0 & 0\\
0 & 1 & 3 & 0\\
0 & 0 & 1 & 3\\
\end{bmatrix}.$$
***
###### Part (b) 
Let 
$$B=\begin{bmatrix}
0 & -9 & 0 & 0\\
1 & 6 & 0 & 0\\
0 & 0 & 0 & -9\\
0 & 0 & 1& 6\\
\end{bmatrix}$$
And notice that $(B-3I)^2=0$. Thus $(x-3)^3$ cannot be the minimal polynomial of $B$. Two matrices are only similar if they share the same invariant factors (and thus the same minimum polynomial), so $A$ and $B$ are not similar.
***
#qual