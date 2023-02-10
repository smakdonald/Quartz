### Problem 6 – Unipotent 4 x 4 Matrices
Let $F$ be a [[Field|field]] and $n$ a positive integer. We say an $n\times n$ matrix $A$ with entries in $F$ is *unipotent* if $A-In$ is [[Nilpotent|nilpotent]] (i.e., $(A-In)^k = 0$ for some $k \geq 1$). For the field $F = \Q$, find (with complete justification) the number of [[Similar Matrices|similarity]] [[Equivalence Class|classes]] of $4\times 4$ unipotent matrices and give an explicit representative for each class.

###### *Proof*.
Let $F=\Q$, $n$ a positive integer, and $A$ a unipotent $4\times 4$ matrix with entries in $F$. Thus $A-I$ is nilpotent. Let $\l$ be an eigenvalue of $A-I$. Then $(A-I)v=\l v$, so $Av-Iv=\l v$ and $Av=\l v+Iv$. As $Iv=v$, we have $Av=\l v+v$ and $Av=(\l+1)v$. 

Notice that as $\l$ is an eigenvalue of $I$, we have $\l +1$ as an eigenvalue of $A$. 

Assume inductively that $\l^{n-1}$ is an eigenvalue of $(A-I)^{n-1}$. Notice $$(A+I)^nv=(A+I)(A+I)^{n-1}v=(A+I)\l^{n-1}v=\l^{n-1}(A+I)v=\l^{n-1}\l=\l^n,$$making $\l$ an eigenvalue of $(A+I)^n$. Thus if $\l$ is an eigenvalue of $A-I$, it is an eigenvalue of $(A-I)^n$ as well. As $(A-I)$ is nilpotent, there exists some $k$ such that $(A-I)^k=0$. This means that $\l^kv=0$. As $v\neq 0$ and $\l^k$ is a scalar in a field (and hence [[Integral Domain|integral domain]]) we have $\l=0$. Thus the only eigenvalue of $(A-I)$ is $0$, meaning that the only eigenvalue of $A$ is $1$. 

Eigenvalues of $A$ correspond to the roots of $\cp_A(x)$ (See: [[Characteristic Polynomial|CharPoly]]), which is a monic quartic polynomial, as $A$ is a $4\times 4$ matrix. Thus $\cp_A(x)=(x-1)^4$, as all roots must be $1$. 

Two matrices are [[Similar Matrices|similar]] if and only if they share the same [[Invariant Factor|invariant factors]]. Given that invariant factors divide $\cp_A(x)$ and each invariant factor must divide the following one, the possible sets of invariant factors for $A$ are the following:
- $\{(x-1)^4\}$,
- $\{(x-1),(x-1)^3\}$,
- $\{(x-1), (x-1), (x-1)^2\}$,
- $\{(x-1)^2, (x-1)^2\}$, and
- $\{(x-1), (x-1), (x-1), (x-1)\}$.
We identify the companion matrices for each possible invariant factor:
$$C(x-1)=\begin{bmatrix} 1 \end{bmatrix},$$$$C((x-1)^2)=C(x^2-2x+1)=\begin{bmatrix} 0 & -1 \\ 1 & 2\end{bmatrix},$$
$$C((x-1)^3)=C(x^3+3x^2+3x-1)=\begin{bmatrix} 0 & 0 & 1 \\ 1 & 0 & -3 \\ 0 & 1 & -3\end{bmatrix},$$ and 
$$C((x-1)^4)=C(x^4-4x^3+6x^2-4x+1)=\begin{bmatrix} 0 & 0 & 0 & -1 \\ 1 & 0 & 0 & 4 \\ 0 & 1 & 0 & -6 \\ 0 & 0 & 1 & 4\end{bmatrix}.$$
We define the following:
1. $B=C((x-1)^4)$, 
2. $C=C(x-1)\oplus C((x-1)^3)$, 
3. $D=C(x-1)\oplus C(x-1)\oplus C((x-1)^2)$, 
4. $E=C((x-1)^2)\oplus C((x-1)^2)$, and 
5. $F=C(x-1)\oplus C(x-1)\oplus C(x-1)\oplus C(x-1)$. 
As each of these matrices is in [[Theorem – Rational Canonical Form|Rational Canonical Form]], they are explicit representatives for each similarity class.
***
#qual