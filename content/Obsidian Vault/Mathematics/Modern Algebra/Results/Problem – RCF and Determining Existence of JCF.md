### Problem 6 – RCF and Determining Existence of JCF
For the matrix $$A=\begin{bmatrix} 0 & -1 & 2 \\ 1 & 0 & 0 \\0 & 1 & -2\end{bmatrix}$$in $\Mat_{3\times3}(\R)$:
(a) Find the [[Theorem – Rational Canonical Form|rational canonical form]] of $A$.
(b) Determine whether or not $A$ has a [[Theorem – Jordan Canonical Form|Jordan canonical form]], and if so, find this form.

##### *Proof*.
###### Part (a)
Notice $\cp_A(x)=\det(A-xI)$. So we have $$\begin{align}\cp_A(x)&=-x\det\begin{bmatrix} -x & 0 \\ 1 & -2-x\end{bmatrix}-(-1)\det\begin{bmatrix} 1 & 0 \\ 0 & -2-x\end{bmatrix}+2\det\begin{bmatrix} 1 & -x \\ 0 & 1\end{bmatrix}\\&=-x(-x(-2-x))+(-2-x)+2(1)\\&=-x^3-2x^2-x\\&-x(x^2+2x+1)\\&=-x(x+1)^2.\end{align}$$Not so bad! 
Now, the invariant factors all divide the characteristic polynomial and must divide the following factor, so our options for sets of invariant factors are the following:
- $\{-x(x+1)^2\}$
- $\{(x+1),-x(x+1)\}$
However, the largest invariant factor is also the minimal polynomial. So we check to see if $-A(A+I)=0$. Luckily, the very first calculation shows that this is not the case. Thus the minimum polynomial is the characteristic polynomial is the only invariant factor of $A$. Thus the RCF of $A$ is $$C(-x^3-2x^2-x)=\begin{bmatrix} 0 & 0 & 0 \\ 1 & 0 & 1 \\0 & 1 & 2\end{bmatrix}.$$
***
###### Part (b)
Luckily for us, $\cp_A(x)$ factors completely into linear terms! So our elementary divisors are $-x$ and $(x+1)^2$. We see $J_1(0)=\begin{bmatrix} 0 \end{bmatrix}$ and $J_2(-1)=\begin{bmatrix} -1 & 0 \\ 1 & -1\end{bmatrix}$, so the Jordan Canonical form of $A$ is $$J=\begin{bmatrix} 0 & 0 & 0 \\ 0 & -1 & 0 \\0 & 1 & -1\end{bmatrix}.$$
***
#qual